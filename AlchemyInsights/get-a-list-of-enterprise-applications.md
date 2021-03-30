---
title: Získání seznamu podnikových aplikací
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404331"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="ab8cb-102">Získání seznamu podnikových aplikací</span><span class="sxs-lookup"><span data-stu-id="ab8cb-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="ab8cb-103">Seznam **podnikových** aplikací (všechny aplikace nebo filtrované podle zobrazovaných názvů, ID, identifikátorů URI identifikátorů atd.) pomocí příkazu Powershellu najdete v tématu [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="ab8cb-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="ab8cb-104">Seznam hlavních objektů služby (všechny objekty nebo filtrované podle ID) pomocí příkazu Powershellu najdete v tématu [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="ab8cb-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="ab8cb-105">Pokud chcete získat **seznam aplikací konfigurovaných samlem, můžou** vám pomoct následující skripty PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="ab8cb-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="ab8cb-106">Každá aplikace, ať už je to aplikace OAuth nebo aplikace SAML (galerie i aplikace mimo galerii), by měly v AAD při registraci vytvořeny dva objekty.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="ab8cb-107">Jeden z nich se nazývá Objekt aplikace a druhý objekt Hlavní služba.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="ab8cb-108">Když vysypáte vlastnosti hlavního objektu služby pomocí PowerShellu, zjistíte, že každá aplikace má určitý počet značek, které jsou s ním spojené, třeba:</span><span class="sxs-lookup"><span data-stu-id="ab8cb-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="ab8cb-109">Aplikace OAuth budou mít značku s názvem **WindowsAzureActiveDirectoryIntegratedApp.**</span><span class="sxs-lookup"><span data-stu-id="ab8cb-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="ab8cb-110">Galerie aplikací SAML by měl značku s názvem **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**</span><span class="sxs-lookup"><span data-stu-id="ab8cb-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="ab8cb-111">Aplikace SAML, které nejsou v galerii, by vlastnily značku s názvem **WindowsAzureActiveDirectoryCustomSingleSignOnApplication.**</span><span class="sxs-lookup"><span data-stu-id="ab8cb-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="ab8cb-112">Proto můžete tyto značky použít a zjistit, jaký druh aplikace to je.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="ab8cb-113">Značka **WindowsAzureActiveDirectoryIntegratedApp je** společná pro všechny typy aplikací.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="ab8cb-114">Následující výstřižek kódu můžete použít k zobrazení seznamu všech aplikací SAML (v galerii i mimo galerii):</span><span class="sxs-lookup"><span data-stu-id="ab8cb-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="ab8cb-115">Další informace najdete v tématu Určení aplikací [s podporou SAML ve službě Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="ab8cb-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="ab8cb-116">**Vyhledání a seznam jenom webových aplikací:** Pomocí následujícího příkazu můžete získat všechny aplikace Azure AD s typem aplikace "Web app/API".</span><span class="sxs-lookup"><span data-stu-id="ab8cb-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="ab8cb-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="ab8cb-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="ab8cb-118">**Vyhledání a seznam samotných nativních aplikací:** Spuštěním následujícího příkazu získáte všechny nativní klientské aplikace (desktopové nebo mobilní zařízení).</span><span class="sxs-lookup"><span data-stu-id="ab8cb-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="ab8cb-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="ab8cb-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="ab8cb-120">**Export všech registrovaných podrobností aplikace Azure AD** do formátu CSV: Následující příkaz exportuje všechny aplikace Azure AD s požadovanými podrobnostmi do souboru CSV:</span><span class="sxs-lookup"><span data-stu-id="ab8cb-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="ab8cb-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="ab8cb-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="ab8cb-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="ab8cb-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="ab8cb-123">**Potřebujete exportovat seznam nepoužívaných aplikací Azure** – sestava auditování</span><span class="sxs-lookup"><span data-stu-id="ab8cb-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="ab8cb-124">Azure AD může zobrazovat protokoly aplikací jenom po dobu 30 dnů za předpokladu, že máte licenci Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="ab8cb-125">Data můžete uchovávat po dobu delší než 30 dnů.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="ab8cb-126">Pomocí rozhraní [API pro vytváření sestav Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) můžete data načíst programově a ukládat je do databáze.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="ab8cb-127">Protokoly auditování můžete také integrovat do systému SIEM třetí strany.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="ab8cb-128">Můžete si taky stáhnout seznam aplikací pro všechny aplikace a vlastněné aplikace v části Azure Active directory>Registrace aplikací>Stáhnout>Všechny aplikace/Vlastněné aplikace.</span><span class="sxs-lookup"><span data-stu-id="ab8cb-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="ab8cb-129">Seznam aplikací přes MS Graph najdete v tématu Seznam aplikací [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) a typ prostředku [aplikace – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="ab8cb-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
