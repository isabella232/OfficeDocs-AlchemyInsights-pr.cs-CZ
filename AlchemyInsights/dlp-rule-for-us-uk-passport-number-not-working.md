---
title: Pravidlo ochrany před únikem pro číslo účtu USA/UK nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679217"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s DLP – čísla v USA/ČR Passport

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP v USA/Spojeném účtu Passport**

Máte problémy s funkcí ochrany před únikem informací **(DLP)** , která nefunguje u obsahu obsahujícího v systému O365 informační typ s informacemi o tom, že je k dispozici v **USA/Spojeném** ? Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co zásada ochrany před úniky hledá při vyhodnocování.
  
Například pro zásady **čísla cestovního pasu pro USA/spojené** s úrovní spolehlivosti 75% jsou následující vyhodnoceny a musí být detekovány, aby se pravidlo spouštěly.
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devět číslic

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devět po sobě jdoucích číslic

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, kontrolní součet neexistuje

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Zásada ochrany před únikem informací je 75%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:

  - Funkce Func_usa_uk_passport najde obsah, který odpovídá vzoru.

  - Najde se klíčové slovo z Keyword_passport.

    Například následující ukázka by mohla vyvolat zásadu **čísla pasu USA/UK** : číslo USA 123456789

Další informace o tom, co je potřeba pro zjištění čísla US/UK pro váš obsah, najdete v tomto článku v této části: [Jaké jsou typy citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .
  
Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  