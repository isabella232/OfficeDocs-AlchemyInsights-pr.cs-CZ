---
title: Řešení problémů s připojením k Azure AD
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
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939912"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Řešení problémů s připojením k Azure AD

1. Pokud registrace zařízení nastavujete poprvé, zkontrolujte, jestli jste v [aplikaci Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) prošly úvodem ke správě zařízení, která vás provede tím, jak dostat zařízení pod kontrolu do Azure AD. 
1. Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, budete [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) muset zajistit, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) a měli jste licenci na prvním místě.
1. Ujistěte se, že máte oprávnění provádět operace v Azure AD. Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD.
1. Pokud chcete provést implementaci připojení k Azure AD, podívejte se na [plánování připojení k Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Další podrobnosti o řešení běžných problémů s připojením k Azure AD najdete v článku Nejčastější dotazy k připojení k [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) a pro zařízení Windows 10 Windows 10 Pro pro vás najdete v tématu Nedaří se připojit počítač k Azure AD – Potřeba upgradovat na – [Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
