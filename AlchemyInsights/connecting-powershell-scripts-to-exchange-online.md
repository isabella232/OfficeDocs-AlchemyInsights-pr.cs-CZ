---
title: Připojení skriptů PowerShellu k Exchangi Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 3a8383a57bc1267311daf03c78841070cca8fb8f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748057"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="219e7-102">Připojení skriptů PowerShellu k Exchangi Online</span><span class="sxs-lookup"><span data-stu-id="219e7-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="219e7-103">Základní ověřování v Exchangi Online se nepoužívá a způsob, jakým se přesměruje, je připojit pomocí ověřování na základě certifikátů pro skripty a bezobslužné úlohy.</span><span class="sxs-lookup"><span data-stu-id="219e7-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="219e7-104">Další informace najdete v tématu o [ověřování v aplikaci jenom pro bezobslužné skripty v modulu EXO v2](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span><span class="sxs-lookup"><span data-stu-id="219e7-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>