---
title: Problémy s vestavěnými počítači
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676875"
---
# <a name="issues-with-onboarding-machines"></a>Problémy s vestavěnými počítači

Je možné, že máte problémy s MDATP službami. Pokud máte přístup k počítači s koncovým uživatelem, postupujte takto:

1. Stáhněte diagnostický nástroj [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) .
2. Extrahujte a spusťte MDATPAnalyzer. cmd.
3. Vyhledejte diagnostický protokol ve složce s názvem MDATPClientAnalyzerResult, což je stejná složka, ve které je nástroj Analyzer stažen.
4. Zkontrolujte soubor protokolu, MDATPClientAnalyzer.txt a najděte problémy s nastavením připojení nebo proxy serveru pro Internet.