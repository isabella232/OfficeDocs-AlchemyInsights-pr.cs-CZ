---
title: Obnovení odstraněného webu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582228"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="9c39d-102">Obnovení odstraněného webu</span><span class="sxs-lookup"><span data-stu-id="9c39d-102">Restore a deleted site</span></span>

<span data-ttu-id="9c39d-103">Když správce odstraní sharepointový web, umístí se do koše kolekce webů, kde je 93 dní před jeho odstraněním.</span><span class="sxs-lookup"><span data-stu-id="9c39d-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="9c39d-104">Chcete-li web obnovit:</span><span class="sxs-lookup"><span data-stu-id="9c39d-104">To restore the site:</span></span>
  
1. <span data-ttu-id="9c39d-105">V novém Centru pro správu SharePointu klikněte na pásu karet na **Koš.**</span><span class="sxs-lookup"><span data-stu-id="9c39d-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="9c39d-106">Zaškrtněte políčko vedle kolekce webů, kterou chcete obnovit.</span><span class="sxs-lookup"><span data-stu-id="9c39d-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="9c39d-107">Klepněte na tlačítko **Obnovit odstraněné položky**.</span><span class="sxs-lookup"><span data-stu-id="9c39d-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="9c39d-108">Pokud chcete obnovit odstraněný komunikační web, můžete použít nové Centrum pro správu SharePointu.</span><span class="sxs-lookup"><span data-stu-id="9c39d-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="9c39d-109">V opačném případě je třeba použít prostředí Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9c39d-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="9c39d-110">Chcete-li obnovit web, který patří do skupiny Microsoft 365, je třeba obnovit skupinu v Centru pro správu Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c39d-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="9c39d-111">Skupiny lze obnovit po dobu 30 dnů po jejich odstranění.</span><span class="sxs-lookup"><span data-stu-id="9c39d-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

