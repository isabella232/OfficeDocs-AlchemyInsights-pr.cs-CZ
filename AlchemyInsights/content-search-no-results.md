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
# <a name="no-results-from-content-searchexports"></a>Vyhledávání a exporty obsahu bez výsledků

Problémy s hledáním a exportem obsahu nevracejí žádná data mohou být způsobena určitým filtrem zabezpečení, který byl nastaven konkrétním správcem, a nekomunikuje ho všem správcům.

Tento problém vyřešíte tak, že zkontrolujete, jestli existují žádné filtry zabezpečení dodržování předpisů, které můžou způsobovat tyto problémy:
1. Připojení k PowerShellu Centrum zabezpečení a dodržování předpisů
2. Spusťte následující rutin:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter – organizace $org