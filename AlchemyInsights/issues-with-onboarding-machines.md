---
title: Problémy s palubními stroji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141364"
---
# <a name="issues-with-onboarding-machines"></a>Problémy s palubními stroji

Můžete mít problémy s onboarding počítače služby MDATP. Pokud máte přístup k počítači koncového uživatele, postupujte takto:

1. Stáhněte si diagnostický nástroj [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)
2. Extrahujte a spusťte soubor MDATPAnalyzer.cmd.
3. Vyhledejte diagnostický protokol ve složce s názvem MDATPClientAnalyzerResult, stejné složce, do které se stahuje nástroj Analyzer.
4. Zkontrolujte soubor protokolu, MDATPClientAnalyzer.txt, abyste našli problémy s připojením nebo nastavením internetového proxy serveru.