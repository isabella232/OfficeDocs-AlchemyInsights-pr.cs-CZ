---
title: Zablokuje mě podmíněný přístup pomocí zařízení připojeného k doméně.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035724"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Zablokuje mě podmíněný přístup pomocí zařízení připojeného k doméně.

**Vysoce doporučené nástroje**

[Nástroj Poradce při potížích s registrací zařízení](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – nástroj, který pomáhá při řešení nejčastějších problémů s registrací zařízení.

[Skript Připojení k registraci testovacího zařízení](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Skript, který pomáhá zajistit, aby zařízení bylo přístup k koncovým bodům registrace zařízení pod systémovým účtem.

[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – Skript, který vám umožní vyhledávat a spravovat zastaralá zařízení ve vašem prostředí.

Tady jsou některé běžné důvody, proč může podmíněný přístup selhávát u zařízení, které se připojilo k doméně (hybridní Azure AD).

1. **Na zařízení není žádná služba Azure AD PRT** – musíte zajistit, aby zařízení měl primární obnovovací token (PRT) Azure AD. Další informace o nástroji PRT najdete v tomto [dokumentu.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Pokud chcete ověřit, jestli máte Azure AD PRT, můžete na zařízení spustit příkaz a ověřit, jestli `dsregcmd/status` se "AzureAdPrt" rovná "ANO".

Pokud "AzureAdPrt" je "NE", zkontrolujte následující:

- Ať už máte **federované** prostředí se službou AD FS a není dostupné z domácích sítí uživatelů : V takovém případě zajistěte, aby byly vaše koncové body "usernamemixed" přístupné z extranetu. Pokud je služba AD FS za sítí VPN, ujistěte se, že se uživatelé připojují k síti VPN, a znovu se přihlaste k zařízení. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Jestli je čip TPM** zařízení vadný, a proto ho nemůže ověřit : Zkontrolujte "tpm.msc", jestli je stav čipu TPM připravený. Pokud ne, spusťte `dsregcmd/leave` a nechte zařízení znovu připojit k Azure AD. Pak to zkuste znovu. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- Používáte poskytovatele identity třetí **strany, který nepodporuje WS-Trust.** Jak je popsáno v našich dokumentech, hybridní zařízení připojená k Azure AD v tomto případě nefungují. Pro podporu prosím pracujte se svým poskytovatelem identity.

2. Uživatelé používají prohlížeč Chrome bez účtů **Windows 10** nebo rozšíření Office Chrome automaticky nepou ít prt na zařízeních připojených ke službě AAD nebo hybridních zařízeních připojených ke službě **AAD:** To vede k selhání všech zásad podmíněného přístupu založených na zařízení s chybovou zprávou "Neregistrované zařízení". Pokud chcete prohlížeč Chrome používat správně, musíte si nainstalovat "Účty Windows 10" nebo "Rozšíření Office pro prohlížeč Chrome uživatelů" přes SCCM nebo Intune. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Pokud není možné rozšíření vzdáleně posunout, upozorní uživatele, aby si ručně nainstalují jedno z výše uvedených rozšíření pro přístup k aplikacím za podmíněným přístupem založeným na zařízeních. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. Zařízení bylo správně připojeno k Hybridní službě Azure AD, ale neúmyslně se odstranilo nebo zakázal, a to buď kvůli změnám synchronizace v **Azure AD Connect,** nebo z webu Azure Portal : Pokud k tomu dojde, objekt zařízení se už nerozpozná jako plně připojené zařízení, i když se stav "AzureAdJoined" a "PRT" na zařízení zobrazí jako platný.

Tento problém vyřešíte tak, že spustíte na dotčených zařízeních a umožníte jim znovu připojit `dsregcmd/leave` se k Azure AD. Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Pokud jsou vaše zařízení ve Windows 10, 1809 update, s VPN/Cloud Proxy a zobrazí se problémy se stavem AzureAdPrt nebo libovolnou aplikací s problémem jednotného přihlašování (outlook se ne připojuje k poštovní schránce, i když jste měli PRT), zkontrolujte, jestli máte tuto opravu [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) nebo dubnovou kumulativní aktualizaci [KB4549949,](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) aby se zabránilo selhání PRT na těchto počítačích.

















