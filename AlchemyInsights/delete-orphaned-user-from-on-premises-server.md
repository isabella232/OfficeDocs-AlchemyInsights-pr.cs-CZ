---
title: Odstranění osamoceného uživatele z místního serveru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197939"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="f6c2c-102">Odstranění osamoceného uživatele z místního serveru</span><span class="sxs-lookup"><span data-stu-id="f6c2c-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="f6c2c-103">Chcete-li odebrat osamoceného uživatele, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="f6c2c-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="f6c2c-104">Vynutit synchronizaci adresářů podle pokynů v části [Co je hybridní identita s Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)</span><span class="sxs-lookup"><span data-stu-id="f6c2c-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="f6c2c-105">Informace o ověření synchronizace adresářů naleznete v [tématu Co je hybridní identita s službou Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="f6c2c-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="f6c2c-106">Pokud synchronizace funguje správně, ale odstranění objektu služby Active Directory se nerozšíří do služby Azure AD, ručně odeberte osamocený objekt pomocí jedné z následujících rutin modulu Azure Active Directory pro prostředí Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f6c2c-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="f6c2c-107">Odstranit-MsolContact</span><span class="sxs-lookup"><span data-stu-id="f6c2c-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="f6c2c-108">Odebrat-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="f6c2c-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="f6c2c-109">Odebrat-Msoluser</span><span class="sxs-lookup"><span data-stu-id="f6c2c-109">Remove-MsolUser</span></span>

    <span data-ttu-id="f6c2c-110">Chcete-li například odebrat osamocené ID uživatele john.smith@contoso.com, původně vytvořené pomocí synchronizace adresářů, spusťte rutinu:</span><span class="sxs-lookup"><span data-stu-id="f6c2c-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="f6c2c-111">Odebrat-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="f6c2c-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>