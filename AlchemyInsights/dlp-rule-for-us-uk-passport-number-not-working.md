---
title: Pravidlo DLP pro americké/britské číslo pasu nefunguje
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004939"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémy s DLP – čísla pasů v USA/Velké Británii

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy SLP s čísly pasů v USA/Spojeném království**

Máte problémy s prevencí ztráty dat **(DLP)** nefunguje u obsahu obsahujícího číslo pasu **USA/Uk** při používání typu citlivých informací pro ochranu před únikem informací v O365? Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co zásady ochrany před únikem informací hledají při jeho vyhodnocení.
  
Například u zásad číslování pasů v **USA/Velké** Británii nakonfigurovaných s úrovní spolehlivosti 75 % se vyhodnocují následující položky a musí být detekovány, aby se pravidlo spouštěl.
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devět číslic

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devět po sobě jdoucích číslic

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, není k dispozici kontrolní součet.

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Zásada ochrany před únikem informací je 75 % přesvědčená o tom, že tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:

  - Funkce Func_usa_uk_passport najde obsah, který odpovídá vzoru.

  - Klíčové slovo z Keyword_passport nalezené.

    Například následující ukázka by se spouštěl pro zásady číslování pasů v **USA/Spojeném** království: Číslo amerického pasu 123456789

Další informace o tom, co je potřeba pro zjištění čísla pasu usa/Spojeného království pro váš obsah, najdete v následující části v tomto článku: Jak vypadají typy citlivých informací pro číslo pasu [USA/Uk Passport](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Informace o tom, co je potřeba pro jiné typy informací, najdete v následujícím článku s použitím jiného typu citlivých [informací:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Co tyto typy citlivých informací vypadají
  