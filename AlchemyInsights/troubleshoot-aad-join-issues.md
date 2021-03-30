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
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="ca6fe-102">Řešení problémů s připojením k Azure AD</span><span class="sxs-lookup"><span data-stu-id="ca6fe-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="ca6fe-103">Pokud registrace zařízení nastavujete poprvé, zkontrolujte, jestli jste si prohlédli Úvod ke správě zařízení v [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) který vás provede tím, jak získat zařízení pod kontrolou do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca6fe-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="ca6fe-104">Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, budete [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) muset zajistit, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) a měli jste licenci na prvním místě.</span><span class="sxs-lookup"><span data-stu-id="ca6fe-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="ca6fe-105">Ujistěte se, že máte oprávnění provádět operace v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca6fe-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="ca6fe-106">Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca6fe-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="ca6fe-107">Pokud chcete provést implementaci připojení k Azure AD, podívejte se na [plánování připojení k Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="ca6fe-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="ca6fe-108">Další podrobnosti o řešení běžných problémů s připojením k Azure AD najdete v článku Nejčastější dotazy k připojení k [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) a pro zařízení s Windows 10 pro najdete v tématu Nedaří se připojit k Azure AD počítač s Windows [10 Pro –](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) potřebujete upgradovat na – komunita Microsoftu</span><span class="sxs-lookup"><span data-stu-id="ca6fe-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
