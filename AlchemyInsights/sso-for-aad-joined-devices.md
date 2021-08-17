---
title: Single-Sign pro Azure Active Directory zařízení připojená
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050003"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Jednotné přihlašování pro Azure Active Directory připojená zařízení

Pokud máte místní prostředí Active Directory (AD) a chcete se připojit k azure AD počítačům připojeným k doméně AD, můžete to udělat pomocí hybridního připojení k Azure AD. [Postupy: Plánování implementace hybridního připojení Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vám poskytne související kroky k implementaci hybridního připojení k Azure AD ve vašem prostředí.

[Konfigurace zařízení připojených ke službě Azure AD pro místní Single-Sign na Windows Hello pro firmy](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problémy s tokenem primární aktualizace (PRT)** Primární obnovovací token (PRT) je klíčový artefakt ověřování Azure AD v Windows 10, Windows Server 2016 a novějších verzích, zařízeních s iOSem a Androidem. Jedná se o webový token JSON (JWT), který je speciálně vydaný zprostředkovatelům tokenů první strany Microsoftu, aby umožnil jednotné přihlašování (SSO) v aplikacích používaných na těchto zařízeních. V části Co je primární [obnovovací token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)poskytneme podrobnosti o tom, jak se prt vydává, používá a chrání na Windows 10 zařízeních.

**WamDefaultSet: ANO a AzureADPrt: ANO** Tato pole označují, jestli se uživatel při přihlášení k zařízení úspěšně ověřil ve službě Azure AD. Pokud jsou hodnoty **NE,** může to být splatné:

- Chybný klíč úložiště v čipu TPM přidruženém k zařízení při registraci (při spouštění zvýšených oprávnění zkontrolujte KeySignTest).
- Alternativní přihlašovací ID
- Http Proxy nebyl nalezen.

Poradce při potížích se zařízeními pomocí příkazu dsregcmd – [stav jednotného přihlašování](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
