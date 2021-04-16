---
title: Obnovení odstraněné veřejné složky
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809432"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="e7040-102">Obnovení odstraněné veřejné složky</span><span class="sxs-lookup"><span data-stu-id="e7040-102">Restore a deleted public folder</span></span>

<span data-ttu-id="e7040-103">**Obnovení odstraněných položek z veřejné složky**:</span><span class="sxs-lookup"><span data-stu-id="e7040-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="e7040-104">Další informace najdete v článku Odstraněné položky v [Outlooku 2016](https://aka.ms/pfrec)se neschová z veřejné složky, která není poštovní.</span><span class="sxs-lookup"><span data-stu-id="e7040-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="e7040-105">**Obnovení odstraněné veřejné složky (libovolného typu):**</span><span class="sxs-lookup"><span data-stu-id="e7040-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="e7040-106">Použijte prosím následující příkaz EXO PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="e7040-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="e7040-107">Syntaxe:</span><span class="sxs-lookup"><span data-stu-id="e7040-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="e7040-108">Příklad: Následující příkaz obnoví podsložku1 a umístěte ji do složky \Parent1:</span><span class="sxs-lookup"><span data-stu-id="e7040-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="e7040-109">Další podrobnosti najdete v článku Obnovení [odstraněné veřejné](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) složky.</span><span class="sxs-lookup"><span data-stu-id="e7040-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
