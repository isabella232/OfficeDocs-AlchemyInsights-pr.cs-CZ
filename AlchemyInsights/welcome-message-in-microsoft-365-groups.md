---
title: Uvítací zpráva ve skupinách Microsoft 365
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
- "1200024"
- "5685"
ms.openlocfilehash: 6c46ba1b2c2c94e21d7c76e45df1d416ba423faf
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806399"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="f8d99-102">Uvítací zpráva ve skupinách Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f8d99-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="f8d99-103">Noví uživatelé, kteří se připojují ke skupině Microsoft 365, dostanou uvítací e-mail, pokud je vlastnost UnifiedGroupWelcomeMessageEnabled pravdivá.</span><span class="sxs-lookup"><span data-stu-id="f8d99-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="f8d99-104">V případě, že chcete uvítací zprávu zakázat, použijte následující [příkaz EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="f8d99-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
