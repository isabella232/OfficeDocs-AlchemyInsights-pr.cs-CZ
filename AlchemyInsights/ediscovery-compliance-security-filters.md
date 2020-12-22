---
title: Při hledání nebo exportu obsahu se nevrátily žádné výsledky.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727216"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="8b33d-102">Při hledání nebo exportu obsahu se nevrátily žádné výsledky.</span><span class="sxs-lookup"><span data-stu-id="8b33d-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="8b33d-103">Pokud máte problémy s následujícími scénáři eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="8b33d-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="8b33d-104">Vyhledávání a export obsahu nevrací žádná data nebo neočekávaná data.</span><span class="sxs-lookup"><span data-stu-id="8b33d-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="8b33d-105">nepovede se hledání nebo export eDiscovery</span><span class="sxs-lookup"><span data-stu-id="8b33d-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="8b33d-106">Může to být kvůli určitým filtrům zabezpečení dodržování předpisů, které byly nastavené konkrétním správcem a nebyly předány všem správcům.</span><span class="sxs-lookup"><span data-stu-id="8b33d-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="8b33d-107">Tento problém vyřešíte tak, že zkontrolujete, jestli existují nějaké filtry zabezpečení dodržování předpisů, které můžou způsobovat tyto problémy:</span><span class="sxs-lookup"><span data-stu-id="8b33d-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="8b33d-108">Připojení k PowerShellu Centrum zabezpečení a dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="8b33d-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8b33d-109">Spusťte následující rutin:</span><span class="sxs-lookup"><span data-stu-id="8b33d-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="8b33d-110">Další informace o filtrech zabezpečení dodržování předpisů najdete v tématu [filtrování oprávnění pro vyhledávání obsahu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search) .</span><span class="sxs-lookup"><span data-stu-id="8b33d-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
