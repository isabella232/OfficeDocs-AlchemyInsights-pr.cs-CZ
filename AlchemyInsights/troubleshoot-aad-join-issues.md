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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404382"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Řešení problémů s připojením k Azure AD

1. Pokud registrace zařízení nastavujete poprvé, zkontrolujte, jestli jste si prohlédli Úvod ke správě zařízení v [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) který vás provede tím, jak získat zařízení pod kontrolou do Azure AD. 
1. Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, budete [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) muset zajistit, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) a měli jste licenci na prvním místě.
1. Ujistěte se, že máte oprávnění provádět operace v Azure AD. Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD.
1. Pokud chcete provést implementaci připojení k Azure AD, podívejte se na [plánování připojení k Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Další podrobnosti o řešení běžných problémů s připojením k Azure AD najdete v článku Nejčastější dotazy k připojení k [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) a pro zařízení s Windows 10 pro najdete v tématu Nedaří se připojit k Azure AD počítač s Windows [10 Pro –](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) potřebujete upgradovat na – komunita Microsoftu
