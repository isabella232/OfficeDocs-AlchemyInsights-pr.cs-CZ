---
title: Vytvoření SharePointového webu
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786558"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="0411c-102">Vytvoření SharePointového webu</span><span class="sxs-lookup"><span data-stu-id="0411c-102">Create a SharePoint site</span></span>

<span data-ttu-id="0411c-103">Vytvářet nebo spravovat weby z [aktivních webů](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) v centru pro správu SharePointu</span><span class="sxs-lookup"><span data-stu-id="0411c-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="0411c-104">Další informace najdete v tématu [Správa webů v novém centru pro správu SharePointu](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="0411c-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="0411c-105">Tipy</span><span class="sxs-lookup"><span data-stu-id="0411c-105">Tips:</span></span>

- <span data-ttu-id="0411c-106">Web se stejnou adresou URL existujícího webu **nelze** vytvořit.</span><span class="sxs-lookup"><span data-stu-id="0411c-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="0411c-107">Pokud jste odstranili web a chcete adresu URL znovu použít, je možné, že odstraněný web na [odstraněných webech](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)pořád existuje.</span><span class="sxs-lookup"><span data-stu-id="0411c-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="0411c-108">K opětovnému použití adresy URL bude nutné tento web trvale odstranit.</span><span class="sxs-lookup"><span data-stu-id="0411c-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="0411c-109">Informace o úplném odebrání webu pomocí PowerShellu najdete v příkladu rutiny [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="0411c-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="0411c-110">Někteří uživatelé nemusí být schopni vytvořit web.</span><span class="sxs-lookup"><span data-stu-id="0411c-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="0411c-111">[Viz Správa vytváření webů v SharePointu Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="0411c-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="0411c-112">Je možné, že se zdá, že se web zablokoval **na delší dobu** .</span><span class="sxs-lookup"><span data-stu-id="0411c-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="0411c-113">Pokud od prvního vystavení tohoto problému uplynulo více než 24 hodin, protokolujte lístek podpory.</span><span class="sxs-lookup"><span data-stu-id="0411c-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="0411c-114">V mnoha případech jsme na řešení ještě pracujeme.</span><span class="sxs-lookup"><span data-stu-id="0411c-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0411c-115">Dokončete řešení alespoň 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="0411c-115">Please give us at least 24 hours to complete a solution.</span></span>
