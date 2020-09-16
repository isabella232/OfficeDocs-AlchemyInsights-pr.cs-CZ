---
title: Odstranění osamoceného uživatele z místního serveru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680128"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="affc4-102">Odstranění osamoceného uživatele z místního serveru</span><span class="sxs-lookup"><span data-stu-id="affc4-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="affc4-103">Pokud chcete odebrat osamoceného uživatele, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="affc4-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="affc4-104">Vynuťte synchronizaci adresářů podle pokynů v části [co je hybridní identita se službou Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="affc4-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="affc4-105">Pokud chcete ověřit synchronizaci adresáře, podívejte se na téma [co je hybridní identita se službou Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="affc4-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="affc4-106">Pokud funkce synchronizace správně funguje, ale odstranění objektu služby Active Directory se nešíří do služby Azure AD, odeberte osamocený objekt ručně pomocí jednoho z následujících rutin Azure Active Directory pro Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="affc4-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="affc4-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="affc4-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="affc4-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="affc4-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="affc4-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="affc4-109">Remove-MsolUser</span></span>

    <span data-ttu-id="affc4-110">Pokud třeba chcete odebrat osamocený ID john.smith@contoso.com, které se původně vytvořilo pomocí synchronizace adresářů, spusťte tuto rutinu:</span><span class="sxs-lookup"><span data-stu-id="affc4-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="affc4-111">Remove-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="affc4-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>