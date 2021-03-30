---
title: Problémy s vlastníkem registrace aplikací
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404294"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="bc446-102">Problémy s vlastníkem registrace aplikací</span><span class="sxs-lookup"><span data-stu-id="bc446-102">App Registration Owner issues</span></span>

<span data-ttu-id="bc446-103">Tady jsou dostupné metody pro přidání objektů zabezpečení jako vlastníků pro registrace aplikací:</span><span class="sxs-lookup"><span data-stu-id="bc446-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="bc446-104">Použití modulu Azure AD PowerShell –</span><span class="sxs-lookup"><span data-stu-id="bc446-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="bc446-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="bc446-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="bc446-106">Používání Azure CLI – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="bc446-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="bc446-107">Reference: [vlastník aplikace az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="bc446-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="bc446-108">Použití ms graphu –</span><span class="sxs-lookup"><span data-stu-id="bc446-108">Using MS Graph -</span></span>

    <span data-ttu-id="bc446-109">Reference: [Přidání vlastníka – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="bc446-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="bc446-110">Použití portálu Azure AD Portal – přejděte na [portal.azure.com](https://portal.azure.com/) > Azure Active directory > Registrace aplikací > Vyberte aplikaci > Vlastníci > Přidat vlastníky</span><span class="sxs-lookup"><span data-stu-id="bc446-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="bc446-111">**Nemůžete zobrazit vaši aplikaci v okně Registrace aplikací, i když jste vlastníkem této aplikace?**</span><span class="sxs-lookup"><span data-stu-id="bc446-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="bc446-112">Vlastníkem aplikace není role správce.</span><span class="sxs-lookup"><span data-stu-id="bc446-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="bc446-113">Pokud je povolené nastavení Omezit přístup k portálu pro správu [Azure AD,](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) bude moct aplikace na portálu registrace aplikací zobrazit jenom správce.</span><span class="sxs-lookup"><span data-stu-id="bc446-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="bc446-114">Aby mohl vlastník zobrazit aplikace, zakažte toto nastavení (Nastavte to na NE) nebo přiřaďte roli správce vlastníkovi jenom pro konkrétní aplikaci.</span><span class="sxs-lookup"><span data-stu-id="bc446-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="bc446-115">K tomu ale budete potřebovat licenci Azure AD Premium P2 a povolit privilegované [správy identit.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="bc446-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
