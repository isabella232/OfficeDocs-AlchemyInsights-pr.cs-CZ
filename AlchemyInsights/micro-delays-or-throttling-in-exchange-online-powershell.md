---
title: Mikrozpoždění a omezování v Exchange Online PowerShellu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702119"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="d7fd9-102">Mikrozpoždění a omezování v Exchange Online PowerShellu</span><span class="sxs-lookup"><span data-stu-id="d7fd9-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="d7fd9-103">Když spustíte skripty a rutiny v Exchangi Online, mohou se zobrazit upozornění „Použito mikrozpoždění“ nebo se objevit zpoždění.</span><span class="sxs-lookup"><span data-stu-id="d7fd9-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="d7fd9-104">Tady je několik návrhů, jak to vyřešit:</span><span class="sxs-lookup"><span data-stu-id="d7fd9-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="d7fd9-105">Spusťte prosím naši diagnostiku, abyste uvolnili zásady omezení PowerShellu vašeho tenanta.</span><span class="sxs-lookup"><span data-stu-id="d7fd9-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="d7fd9-106">Toto řešení vyřeší problém většinou.</span><span class="sxs-lookup"><span data-stu-id="d7fd9-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="d7fd9-107">Pokud se problém stále nevyřeší, použijte [modul PowerShellu Exchange Online verze 2,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)který zahrnuje cmdlety, které jsou založené na rozhraní REST API a jsou podstatně výkonnější.</span><span class="sxs-lookup"><span data-stu-id="d7fd9-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="d7fd9-108">Může to být skvělé řešení pro velké množství často používaných rutin Get-.</span><span class="sxs-lookup"><span data-stu-id="d7fd9-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="d7fd9-109">Pokud potřebujete používat cmdlety, které nejsou zahrnuté v modulu v2, přečtěte si prosím téma Spouštění rutin [PowerShellu](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)pro velký počet uživatelů v Office 365 , který hovoří o tom, jak se v Exchange Online obekat omezení PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="d7fd9-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
