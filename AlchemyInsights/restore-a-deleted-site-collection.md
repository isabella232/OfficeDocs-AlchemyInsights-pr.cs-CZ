---
title: Obnovení odstraněného webu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692036"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="cae4e-102">Obnovení odstraněného webu</span><span class="sxs-lookup"><span data-stu-id="cae4e-102">Restore a deleted site</span></span>

<span data-ttu-id="cae4e-103">Když správce odstraní SharePointový web, umístí se do koše kolekce webů, kde je po dobu 93 dní před trvalým odstraněním trvale odstraněný.</span><span class="sxs-lookup"><span data-stu-id="cae4e-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="cae4e-104">Obnovení webu:</span><span class="sxs-lookup"><span data-stu-id="cae4e-104">To restore the site:</span></span>
  
1. <span data-ttu-id="cae4e-105">V novém centru pro správu SharePointu klikněte na pásu karet na **Koš** .</span><span class="sxs-lookup"><span data-stu-id="cae4e-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="cae4e-106">Zaškrtněte políčko vedle kolekce webů, kterou chcete obnovit.</span><span class="sxs-lookup"><span data-stu-id="cae4e-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="cae4e-107">Klikněte na **Obnovit odstraněné položky**.</span><span class="sxs-lookup"><span data-stu-id="cae4e-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="cae4e-108">Pokud chcete obnovit odstraněný komunikační web, můžete použít nové centrum pro správu SharePointu.</span><span class="sxs-lookup"><span data-stu-id="cae4e-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="cae4e-109">V opačném případě potřebujete použít Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cae4e-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="cae4e-110">Pokud chcete obnovit web, který patří do skupiny Microsoft 365, musíte obnovit skupinu v centru pro správu Exchange.</span><span class="sxs-lookup"><span data-stu-id="cae4e-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="cae4e-111">Skupiny se dají obnovit po dobu 30 dnů po jejich odstranění.</span><span class="sxs-lookup"><span data-stu-id="cae4e-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

