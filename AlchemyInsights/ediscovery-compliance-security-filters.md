---
title: Během vyhledávání a exportu obsahu se nevrátily žádné výsledky.
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101259"
---
# <a name="no-results-returned-during-content-searchexport"></a>Během vyhledávání a exportu obsahu se nevrátily žádné výsledky.

Pokud máte problémy s následujícími scénáři eDiscovery:

- Funkce Vyhledávání a export obsahu nevrátí žádná data ani neočekávaná data.
- Hledání nebo export eDiscovery se nezdaří.

Může to být způsobeno určitými filtry zabezpečení dodržování předpisů, které byly nasaovány určitým správcem a nebyly oznámeny všem správcům.

Tento problém vyřešíte tak, že zkontrolujete, jestli existují nějaké filtry zabezpečení dodržování předpisů, které těmto problémům mohou způsobovat:

1. Připojení do Centra zabezpečení a dodržování předpisů PowerShell
2. Spusťte následující commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Další informace o filtrech zabezpečení dodržování předpisů najdete v tématu [Filtrování oprávnění pro vyhledávání obsahu.](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
