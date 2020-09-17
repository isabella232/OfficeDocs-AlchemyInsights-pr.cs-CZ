---
title: Vytvoření SharePointového webu
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806932"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="008fc-102">Vytvoření SharePointového webu</span><span class="sxs-lookup"><span data-stu-id="008fc-102">Create a SharePoint site</span></span>

<span data-ttu-id="008fc-103">Vytvářet nebo spravovat weby z [aktivních webů](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) v centru pro správu SharePointu</span><span class="sxs-lookup"><span data-stu-id="008fc-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="008fc-104">Další informace najdete v tématu [Správa webů v novém centru pro správu SharePointu](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="008fc-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="008fc-105">Tipy</span><span class="sxs-lookup"><span data-stu-id="008fc-105">Tips:</span></span>

- <span data-ttu-id="008fc-106">Web se stejnou adresou URL existujícího webu **nelze** vytvořit.</span><span class="sxs-lookup"><span data-stu-id="008fc-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="008fc-107">Pokud jste odstranili web a chcete adresu URL znovu použít, je možné, že odstraněný web na [odstraněných webech](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)pořád existuje.</span><span class="sxs-lookup"><span data-stu-id="008fc-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="008fc-108">K opětovnému použití adresy URL bude nutné tento web trvale odstranit.</span><span class="sxs-lookup"><span data-stu-id="008fc-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="008fc-109">Informace o úplném odebrání webu pomocí PowerShellu najdete v příkladu rutiny [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="008fc-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="008fc-110">Někteří uživatelé nemusí být schopni vytvořit web.</span><span class="sxs-lookup"><span data-stu-id="008fc-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="008fc-111">[Viz Správa vytváření webů v SharePointu Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="008fc-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="008fc-112">Je možné, že se zdá, že se web zablokoval **na delší dobu** .</span><span class="sxs-lookup"><span data-stu-id="008fc-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="008fc-113">Pokud od prvního vystavení tohoto problému uplynulo více než 24 hodin, protokolujte lístek podpory.</span><span class="sxs-lookup"><span data-stu-id="008fc-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="008fc-114">V mnoha případech jsme na řešení ještě pracujeme.</span><span class="sxs-lookup"><span data-stu-id="008fc-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="008fc-115">Dokončete řešení alespoň 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="008fc-115">Please give us at least 24 hours to complete a solution.</span></span>
