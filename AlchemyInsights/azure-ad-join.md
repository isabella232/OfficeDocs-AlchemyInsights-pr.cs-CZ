---
title: Azure Active Directory připojení
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
- "9890"
ms.openlocfilehash: 6a772d7bad7f00940ee45a2a2e6860321cefe331
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331488"
---
# <a name="azure-active-directory-join"></a>Azure Active Directory připojení

1. Pokud registrace zařízení nastavujete poprvé, ujistěte se, že jste si v aplikaci Azure Active Directory prohlédli Úvod ke správě [zařízení,](https://docs.microsoft.com/azure/active-directory/devices/overview) který vás provede tím, jak získat zařízení pod kontrolou do Azure AD. 
1. Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, budete [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) muset zajistit, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) a měli jste licenci na prvním místě.
1. Ujistěte se, že máte oprávnění provádět operace v Azure AD. Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD.
1. Pokud chcete provést implementaci připojení k Azure AD, podívejte se na [plánování připojení k Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Další podrobnosti o řešení běžných problémů s připojením k Azure AD najdete v článku Nejčastější dotazy k připojení k [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq) a pro zařízení Windows 10 pro, najdete v článku Nedaří se připojit se k Azure AD na počítač Windows 10 Pro – potřebujete upgradovat na – [Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).
