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
# <a name="no-results-from-content-searchexports"></a>Žádné výsledky z vyhledávání nebo exportu obsahu

Problémy s vyhledáváním nebo exportem obsahu, které nevrací žádná data, mohou být způsobené určitým filtrem zabezpečení dodržování předpisů, který nasaul konkrétní správce a nesvědí je všem správcům.

Pokud to chcete vyřešit, zkontrolujte, jestli nejsou nějaké filtry zabezpečení dodržování předpisů, které by to mohlo způsobovat:
1. Připojení k Centru zabezpečení a dodržování předpisů PowerShell
2. Spusťte následující commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organizace $org