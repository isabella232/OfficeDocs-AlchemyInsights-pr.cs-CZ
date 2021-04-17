---
title: Hledání obsahu bez výsledků
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816841"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="efbf7-102">Žádné výsledky z vyhledávání nebo exportu obsahu</span><span class="sxs-lookup"><span data-stu-id="efbf7-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="efbf7-103">Problémy s vyhledáváním nebo exportem obsahu, které nevrací žádná data, mohou být způsobené určitým filtrem zabezpečení dodržování předpisů, který nasaul konkrétní správce a nesvědí je všem správcům.</span><span class="sxs-lookup"><span data-stu-id="efbf7-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="efbf7-104">Pokud to chcete vyřešit, zkontrolujte, jestli nejsou nějaké filtry zabezpečení dodržování předpisů, které by to mohlo způsobovat:</span><span class="sxs-lookup"><span data-stu-id="efbf7-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="efbf7-105">Připojení k Centru zabezpečení a dodržování předpisů PowerShell</span><span class="sxs-lookup"><span data-stu-id="efbf7-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="efbf7-106">Spusťte následující commandlets:</span><span class="sxs-lookup"><span data-stu-id="efbf7-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="efbf7-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="efbf7-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="efbf7-108">Get-ComplianceSecurityFilter -Organizace $org</span><span class="sxs-lookup"><span data-stu-id="efbf7-108">Get-ComplianceSecurityFilter -Organization $org</span></span>