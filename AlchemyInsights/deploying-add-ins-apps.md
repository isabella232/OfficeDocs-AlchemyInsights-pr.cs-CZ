---
title: Nasazení doplňků pro Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "52124964"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="9b078-102">Nasazení doplňků pro Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="9b078-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="9b078-103">Centralizované nasazení je doporučený způsob nasazení doplňků Office uživatelům a skupinám ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9b078-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="9b078-104">Pokud chcete nasadit doplňky, postupujte podle následujících kroků:</span><span class="sxs-lookup"><span data-stu-id="9b078-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="9b078-105">**Poznámka:** Pokud chcete nainstalovat doplňky pro Office uživatele, podívejte se na informace v tématu Zobrazení, správa a instalace doplňků v [Office aplikacích](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span><span class="sxs-lookup"><span data-stu-id="9b078-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="9b078-106">Ujistěte se také, že je povolené individuální Office doplňků pro Store.</span><span class="sxs-lookup"><span data-stu-id="9b078-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="9b078-107">Zajistěte, aby vaše prostředí splňovalo požadavky na nasazení doplňků pomocí centralizovaného nasazení.</span><span class="sxs-lookup"><span data-stu-id="9b078-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="9b078-108">Podrobnosti najdete v tématu [Požadavky](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="9b078-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="9b078-109">Pokud chcete **Nastavení**  >  **doplňky,** přejděte na Microsoft 365 aplikace Získat aplikace v Centru pro  >   správu.</span><span class="sxs-lookup"><span data-stu-id="9b078-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="9b078-110">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="9b078-110">Notes:</span></span> 

- <span data-ttu-id="9b078-111">Integrované aplikace vyžadují, aby správce měl oprávnění globálního správce nebo Exchange správce.</span><span class="sxs-lookup"><span data-stu-id="9b078-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="9b078-112">Při nasazování doplňků více uživatelům doporučujeme zadání provést pomocí skupin místo jednotlivých uživatelů.</span><span class="sxs-lookup"><span data-stu-id="9b078-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="9b078-113">Podrobnosti najdete v tématu Důležité informace při přiřazování doplňku uživatelům [a skupinám.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="9b078-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="9b078-114">Centralizované nasazení nepodporuje uživatele ve vnořených skupinách nebo skupinách, které mají nadřazené skupiny.</span><span class="sxs-lookup"><span data-stu-id="9b078-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="9b078-115">Podrobnosti najdete v tématu [Přiřazení uživatelů a skupin](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="9b078-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="9b078-116">Ujistěte se, že je pro uživatele povolená služba správy aplikací Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a').</span><span class="sxs-lookup"><span data-stu-id="9b078-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="9b078-117">Podrobnosti najdete v tématu [Konfigurace vlastností aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="9b078-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="9b078-118">Pokud máte problémy s nasazením doplňků pomocí integrovaných aplikací, zkuste nasazení pomocí [doplňků](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="9b078-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="9b078-119">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="9b078-119">For more information, see:</span></span>

<span data-ttu-id="9b078-120">[Nasazení doplňků v Centru pro správu](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Správa doplňků v Centru pro správu](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Použití rutin PowerShellu pro centralizované](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) nasazení ke správě doplňků 
 [Publikování Office pomocí Centralizovaného nasazení prostřednictvím Centra Microsoft 365 pro správu](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Poradce při potížích:](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) Uživatel neuvidí doplňky 
 [Odstraňování chyb uživatelů Office doplňky](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="9b078-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>