---
title: Nastavení nebo změna oprávnění veřejné složky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789200"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="b36ee-102">Oprávnění a veřejné složky</span><span class="sxs-lookup"><span data-stu-id="b36ee-102">Permissions and Public Folders</span></span>

<span data-ttu-id="b36ee-103">Oprávnění k veřejným složkám můžete změnit pomocí Outlooku, Centra pro správu Exchange (EAC) nebo PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="b36ee-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="b36ee-104">Pokyny k Outlooku najdete [kliknutím sem.](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)</span><span class="sxs-lookup"><span data-stu-id="b36ee-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="b36ee-105">Pokyny k EAC najdete v [tomto](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) článku.</span><span class="sxs-lookup"><span data-stu-id="b36ee-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="b36ee-106">Pokyny k použití [](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) příkazového Add-PublicFolderClientPermission powershellu najdete v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="b36ee-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="b36ee-107">Pokud potřebujete pokyny pro připojení k Exchange Powershellu, klikněte [sem.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)</span><span class="sxs-lookup"><span data-stu-id="b36ee-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="b36ee-108">Pokud **externí uživatelé nemůžou posílat e-maily** do veřejné složky s podporou pošty , může to být tím, že ve veřejné složce chybí oprávnění potřebná k externímu doručování e-mailů.</span><span class="sxs-lookup"><span data-stu-id="b36ee-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="b36ee-109">Tento problém můžete vyřešit podle pokynů v [Outlooku nebo](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)pokynů v PowerShellu [tady](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="b36ee-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

