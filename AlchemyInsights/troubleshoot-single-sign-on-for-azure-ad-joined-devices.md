---
title: Řešení potíží s jednotným přihlašováním pro zařízení připojená k Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035106"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Řešení potíží s jednotným přihlašováním pro zařízení připojená k Azure AD

Pokud máte místní prostředí Active Directory (AD) a chcete se připojit k azure AD počítačům připojeným k doméně AD, můžete to udělat pomocí hybridního připojení k Azure AD. [Postupy: Plánování implementace připojení k hybridní](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) službě Azure Active Directory vám poskytne související kroky k implementaci hybridního připojení k Azure AD ve vašem prostředí.

Další informace najdete v tématu Konfigurace zařízení připojených [ke službě Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)pro místní Single-Sign v systému Windows Hello pro firmy .

**Problémy s tokenem primární aktualizace (PRT)**

Token primární aktualizace (PRT) je klíčový artefakt ověřování Azure AD ve Windows 10, Windows Serveru 2016 a novějších verzích, zařízeních s iOS a Androidem. Jedná se o webový token JSON (JWT), který je speciálně vydaný zprostředkovatelům tokenů první strany Microsoftu, aby umožnil jednotné přihlašování (SSO) v aplikacích používaných na těchto zařízeních. Podrobnosti o tom, jak se prt vydává, používá a chrání na zařízeních s Windows 10, najdete v tématu Co je token [primární aktualizace?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: ANO a AzureADPrt: ANO**

Tato pole označují, jestli se uživatel při přihlášení k zařízení úspěšně ověřil ve službě Azure AD. Pokud jsou hodnoty **NE,** může to být kvůli:

- Chybný klíč úložiště v čipu TPM přidruženém k zařízení při registraci (při spouštění zvýšených oprávnění zkontrolujte KeySignTest)
- Alternativní přihlašovací ID
- Http Proxy nebyl nalezen.

Informace o řešení potíží se zařízeními pomocí příkazu dsregcmd najdete v tématu [Stav jednotného přihlašování](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
