---
title: Pravidlo DLP pro americké číslo bankovního účtu nefunguje
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005011"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problémy SLP s čísly bankovních účtů v USA

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy SLP s čísly bankovních účtů v USA**

Máte problémy s prevencí ztráty dat **(DLP)**  nefunguje u obsahu obsahujícího číslo bankovního účtu USA při použití typu citlivých informací DLP v O365? Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co zásady ochrany před únikem informací hledají při jeho vyhodnocení.
  
Například u zásad čísla bankovního účtu v USA nakonfigurovaných s úrovní spolehlivosti 85 % se vyhodnocují následující položky **a** pravidlo musí být detekováno, aby se pravidlo spouštěl takto:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 číslic

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 po sobě jdoucích číslic.

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, není k dispozici kontrolní součet.

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zásada ochrany před únikem informací je 75 % přesvědčená o tom, že tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:

  - Funkce regulárního výrazu Regex_usa_bank_account_number najde obsah, který odpovídá vzoru.

  - Klíčové slovo Keyword_usa_Bank_Account nalezené.

    Například následující ukázka by se spouštěl pro zásadu **Číslo** bankovního účtu USA: Kontrola 78344011

Další informace o tom,  co je potřeba pro zjištění čísla bankovního účtu USA pro váš obsah, najdete v následující části v tomto článku: Jak vypadají typy citlivých informací pro americké číslo bankovního [účtu.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Informace o tom, co je potřeba pro jiné typy informací, najdete v následujícím článku s použitím jiného typu citlivých [informací:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Co tyto typy citlivých informací vypadají
  