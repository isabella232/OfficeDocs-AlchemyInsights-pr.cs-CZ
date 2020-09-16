---
title: Uvítací zpráva ve skupinách Microsoft 365
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
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725832"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="c79ad-102">Uvítací zpráva ve skupinách Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c79ad-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="c79ad-103">Noví uživatelé, kteří se připojují ke skupině Microsoft 365, obdrží uvítací e-mail, pokud má vlastnost "UnifiedGroupWelcomeMessageEnabled" hodnotu true.</span><span class="sxs-lookup"><span data-stu-id="c79ad-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="c79ad-104">Pokud chcete uvítací zprávu zakázat, použijte následující [EXO příkaz PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) :</span><span class="sxs-lookup"><span data-stu-id="c79ad-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
