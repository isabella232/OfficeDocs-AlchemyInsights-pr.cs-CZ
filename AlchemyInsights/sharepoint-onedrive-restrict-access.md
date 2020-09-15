---
title: Omezení přístupu v SharePointu nebo OneDrivu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700448"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="365af-102">Omezení přístupu v SharePointu nebo OneDrivu</span><span class="sxs-lookup"><span data-stu-id="365af-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="365af-103">Existuje mnoho způsobů, jak omezit přístup ke službám SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="365af-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="365af-104">Níže jsou uvedené různé metody omezení přístupu.</span><span class="sxs-lookup"><span data-stu-id="365af-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="365af-105">**Omezení oprávnění**</span><span class="sxs-lookup"><span data-stu-id="365af-105">**Permission Restriction**</span></span>

<span data-ttu-id="365af-106">V SharePointu Online a OneDrivu pro firmy omezujeme přístup k položkám, jako jsou weby, soubory a složky, udělením přístupu pouze k těmto skupinám nebo jednotlivcům, kteří by měli mít přístup.</span><span class="sxs-lookup"><span data-stu-id="365af-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="365af-107">Přizpůsobení oprávnění pro SharePointový seznam nebo knihovnu</span><span class="sxs-lookup"><span data-stu-id="365af-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="365af-108">Přizpůsobení oprávnění SharePointového webu</span><span class="sxs-lookup"><span data-stu-id="365af-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="365af-109">Změna oprávnění u podsložky</span><span class="sxs-lookup"><span data-stu-id="365af-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="365af-110">Řízení přístupu z nespravovaných zařízení</span><span class="sxs-lookup"><span data-stu-id="365af-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="365af-111">Jako SharePointový nebo globální správce můžete blokovat nebo omezit přístup k obsahu SharePointu a OneDrivu z nespravovaných zařízení (což není hybridní služba AD spojená nebo kompatibilní v Intune).</span><span class="sxs-lookup"><span data-stu-id="365af-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="365af-112">**Omezení síťového umístění**</span><span class="sxs-lookup"><span data-stu-id="365af-112">**Network Location Restriction**</span></span>

<span data-ttu-id="365af-113">Jako správce IT můžete řídit přístup k prostředkům SharePoint a OneDrive na základě definovaných síťových umístění, kterým důvěřujete.</span><span class="sxs-lookup"><span data-stu-id="365af-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="365af-114">Toto se označuje také jako zásady založené na poloze.</span><span class="sxs-lookup"><span data-stu-id="365af-114">This is also known as location-based policy.</span></span> <span data-ttu-id="365af-115">Další informace najdete v tématu [řízení přístupu k datům SharePointu Online a OneDrivu na základě síťového umístění](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .</span><span class="sxs-lookup"><span data-stu-id="365af-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="365af-116">**Omezení uzamčení webu**</span><span class="sxs-lookup"><span data-stu-id="365af-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="365af-117">V SharePointu Online můžete kolekci webů uzamknout, takže nikdo nemá přístup.</span><span class="sxs-lookup"><span data-stu-id="365af-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="365af-118">To se nastavuje prostřednictvím PowerShellu a [prostředí SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocí vlastnosti [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="365af-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="365af-119">**Zakázání vytváření webů a podřízených webů uživateli**</span><span class="sxs-lookup"><span data-stu-id="365af-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="365af-120">Jako správce SharePointu nebo globální správce můžete uživatelům dovolit vytvářet a spravovat vlastní weby služby SharePoint, určit, jaký typ webů můžou vytvářet, a určit umístění webů.</span><span class="sxs-lookup"><span data-stu-id="365af-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="365af-121">Další informace najdete v tématu [Správa vytváření webů v SharePointu Online](https://docs.microsoft.com/sharepoint/manage-site-creation) .</span><span class="sxs-lookup"><span data-stu-id="365af-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

