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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677684"
---
# <a name="no-results-returned-during-content-searchexport"></a>Při hledání nebo exportu obsahu se nevrátily žádné výsledky.

Pokud máte problémy s následujícími scénáři eDiscovery:

- Vyhledávání a export obsahu nevrací žádná data nebo neočekávaná data.
- nepovede se hledání nebo export eDiscovery

Může to být způsobeno některými filtry zabezpečení dodržování předpisů, které byly nastavené konkrétním správcem a nebyly předány všem správcům.

Tento problém vyřešíte tak, že zkontrolujete, jestli existují nějaké filtry zabezpečení dodržování předpisů, které můžou způsobovat tyto problémy:

1. Připojení k PowerShellu Centrum zabezpečení a dodržování předpisů
2. Spusťte následující rutin:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Další informace o filtrech zabezpečení dodržování předpisů najdete v tématu [filtrování oprávnění pro vyhledávání obsahu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search) .
