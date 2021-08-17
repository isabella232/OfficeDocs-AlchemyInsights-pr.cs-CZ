---
title: Azure Active Directory spojení
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
ms.openlocfilehash: 9e08d6c2a4553e395b5206816f29471118bb3b286e669c0b2d07a740e2a3c749
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894544"
---
# <a name="azure-active-directory-join"></a>Azure Active Directory spojení

1. Pokud registrace zařízení nastavujete poprvé, ujistěte se, že jste si v aplikaci Azure Active Directory prohlédli Úvod ke správě [zařízení,](https://docs.microsoft.com/azure/active-directory/devices/overview) který vás provede tím, jak získat zařízení pod kontrolou do Azure AD. 
1. Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, budete [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) muset zajistit, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) a měli jste licenci na prvním místě.
1. Ujistěte se, že máte oprávnění provádět operace v Azure AD. Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD.
1. Pokud chcete provést implementaci připojení k Azure AD, podívejte se na [plánování připojení k Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Další podrobnosti o řešení běžných problémů s připojením k Azure AD najdete v článku Nejčastější dotazy k připojení k [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq) a pro zařízení Windows 10 pro vás najdete v tématu Nedaří se připojit k Azure AD na počítač Windows 10 Pro – potřebujete upgradovat na – [Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).
