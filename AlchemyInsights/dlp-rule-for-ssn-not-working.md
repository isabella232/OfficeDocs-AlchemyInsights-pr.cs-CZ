---
title: Pravidlo DLP pro SSN nefunguje
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004975"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problémy s DLP s čísly sociálního zabezpečení

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP se sítěmi SSN**

Máte problémy s prevencí ztráty dat **(DLP)** nefunguje u obsahu obsahujícího číslo sociálního zabezpečení **(SSN)** při použití citlivého typu informací v Microsoft 365? Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co zásady ochrany před únikem informací hledají. 
  
Například u zásad SSN nakonfigurovaných s úrovní spolehlivosti 85 % se vyhodnocují následující položky a musí být rozpoznány, aby se pravidlo spouštěly:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, které mohou být v formátovaném nebo neformátovaném vzoru

- **[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Čtyři funkce vypadají pro sítě SSN ve čtyřech různých vzorcích:

  - Func_ssn najde sítě SSN se silným formátováním před 2011, které jsou formátované pomlčkami nebo mezerami (ddd-dd-dddd NEBO ddd dddd)

  - Func_unformatted_ssn najde sítě SSN se silným formátováním před rokem 2011, které nejsou formátované jako devět po sobě jdoucích číslic (dddddddddd)

  - Func_randomized_formatted_ssn najde sítě SSN po roce 2011, které jsou formátované pomlčkami nebo mezerami (ddd-dd-dddd NEBO ddd dddd)

  - Func_randomized_unformatted_ssn najde sítě SSN po roce 2011, které nejsou formátované jako devět po sobě jdoucích číslic (ddddddddd)

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, není k dispozici kontrolní součet.

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Zásada ochrany před únikem informací je z 85 % přesvědčená, že tento typ citlivých informací zjistila, pokud v blízkosti 300 znaků:

  - Funkce [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) najde obsah, který odpovídá vzoru.

  - Je nalezeno [klíčové Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) z aplikace. Mezi klíčová slova patří:  *Sociální zabezpečení, Sociální zabezpečení#, Soc Sec ,SSN*  . Například následující ukázka by se spouštěl pro zásadu SSN DLP: **SSN: 489-36-8350**
  
Další informace o tom, co je potřeba pro zjištění sítí SAN pro váš obsah, najdete v následující části v tomto článku: Co vypadají typy citlivých informací pro [sítě SAN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Informace o tom, co je potřeba pro jiné typy informací, najdete v následujícím článku s použitím jiného typu citlivých [informací:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Co tyto typy citlivých informací vypadají
  