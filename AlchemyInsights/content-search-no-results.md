---
title: Hledání obsahu – žádné výsledky
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680640"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="dbe2a-102">Vyhledávání a exporty obsahu bez výsledků</span><span class="sxs-lookup"><span data-stu-id="dbe2a-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="dbe2a-103">Problémy s hledáním a exportem obsahu nevracejí žádná data mohou být způsobena určitým filtrem zabezpečení, který byl nastaven konkrétním správcem, a nekomunikuje ho všem správcům.</span><span class="sxs-lookup"><span data-stu-id="dbe2a-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="dbe2a-104">Tento problém vyřešíte tak, že zkontrolujete, jestli existují žádné filtry zabezpečení dodržování předpisů, které můžou způsobovat tyto problémy:</span><span class="sxs-lookup"><span data-stu-id="dbe2a-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="dbe2a-105">Připojení k PowerShellu Centrum zabezpečení a dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="dbe2a-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="dbe2a-106">Spusťte následující rutin:</span><span class="sxs-lookup"><span data-stu-id="dbe2a-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="dbe2a-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="dbe2a-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="dbe2a-108">Get-ComplianceSecurityFilter – organizace $org</span><span class="sxs-lookup"><span data-stu-id="dbe2a-108">Get-ComplianceSecurityFilter -Organization $org</span></span>