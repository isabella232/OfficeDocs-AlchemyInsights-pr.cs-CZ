---
title: Mikrozpoždění a omezování v Exchange Online PowerShellu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743907"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="1927e-102">Mikrozpoždění a omezování v Exchange Online PowerShellu</span><span class="sxs-lookup"><span data-stu-id="1927e-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="1927e-103">Když spustíte skripty a rutiny v Exchangi Online, mohou se zobrazit upozornění „Použito mikrozpoždění“ nebo se objevit zpoždění.</span><span class="sxs-lookup"><span data-stu-id="1927e-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="1927e-104">Tady jsou dva návrhy, které se toho týkají:</span><span class="sxs-lookup"><span data-stu-id="1927e-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="1927e-105">Můžete zkusit použít [modul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), který obsahuje rutiny založené na rozhraní REST API a je výrazně výkonnější.</span><span class="sxs-lookup"><span data-stu-id="1927e-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="1927e-106">Může to být skvělé řešení pro velké množství často používaných rutin Get-.</span><span class="sxs-lookup"><span data-stu-id="1927e-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="1927e-107">Pokud potřebujete použít rutiny, které ještě nejsou zavedené v modulu v2, přečtěte si téma [Spuštění rutin PowerShellu pro velké počty uživatelů v Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), které se zabývá tím, jak obejít očekávané limity omezování PowerShellu v Exchangi Online.</span><span class="sxs-lookup"><span data-stu-id="1927e-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
