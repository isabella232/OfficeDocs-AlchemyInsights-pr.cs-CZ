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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057995"
---
# <a name="no-results-from-content-searchexports"></a>Žádné výsledky z vyhledávání nebo exportu obsahu

Problémy s vyhledáváním nebo exportem obsahu, které nevrací žádná data, mohou být způsobené určitým filtrem zabezpečení dodržování předpisů, který nasaul konkrétní správce a nesvědí je všem správcům.

Pokud to chcete vyřešit, zkontrolujte, jestli nejsou nějaké filtry zabezpečení dodržování předpisů, které by to mohlo způsobovat:
1. Připojení do Centra zabezpečení a dodržování předpisů PowerShell
2. Spusťte následující commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organizace $org