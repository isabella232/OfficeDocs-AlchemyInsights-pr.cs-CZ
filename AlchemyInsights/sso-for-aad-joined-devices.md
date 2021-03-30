---
title: Single-Sign pro zařízení připojená k Azure Active Directory
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
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404362"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Jednotné přihlašování pro zařízení připojená k Azure Active Directory

Pokud máte místní prostředí Active Directory (AD) a chcete se připojit k azure AD počítačům připojeným k doméně AD, můžete to udělat pomocí hybridního připojení k Azure AD. [Postupy: Plánování implementace připojení k hybridní](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) službě Azure Active Directory vám poskytne související kroky k implementaci hybridního připojení k Azure AD ve vašem prostředí.

[Konfigurace zařízení připojených ke službě Azure AD pro místní Single-Sign v systému Windows Hello pro firmy](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problémy s tokenem primární aktualizace (PRT)** Token primární aktualizace (PRT) je klíčový artefakt ověřování Azure AD ve Windows 10, Windows Serveru 2016 a novějších verzích, zařízeních s iOS a Androidem. Jedná se o webový token JSON (JWT), který je speciálně vydaný zprostředkovatelům tokenů první strany Microsoftu, aby umožnil jednotné přihlašování (SSO) v aplikacích používaných na těchto zařízeních. [V části Co je](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)token primární aktualizace? poskytneme podrobnosti o tom, jak se na zařízeních s Windows 10 vydává, používá a chrání PRT.

**WamDefaultSet: ANO a AzureADPrt: ANO** Tato pole označují, jestli se uživatel při přihlášení k zařízení úspěšně ověřil ve službě Azure AD. Pokud jsou hodnoty **NE,** může to být splatné:

- Chybný klíč úložiště v čipu TPM přidruženém k zařízení při registraci (při spouštění zvýšených oprávnění zkontrolujte KeySignTest).
- Alternativní přihlašovací ID
- Http Proxy nebyl nalezen.

Poradce při potížích se zařízeními pomocí příkazu dsregcmd – [stav jednotného přihlašování](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
