---
title: Pravidlo ochrany před únikem číslo bankovního účtu USA nefunguje
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679289"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problémy s DLP s čísly bankovních účtů USA

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP s čísly bankovních účtů USA**

Máte problémy s funkcí ochrany před únikem informací **(DLP)** , která nefunguje u obsahu obsahujícího **číslo bankovního účtu USA** při používání informačního typu s citlivými informacemi o DLP v O365? Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co zásada ochrany před úniky hledá při vyhodnocování.
  
Například pro zásady **bankovního účtu US** , která je nakonfigurovaná s úrovní spolehlivosti 85%, se vyhodnocuje následující hodnota, která se má pro pravidlo aktivovat:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 číslic

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 po sobě jdoucích číslic.

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, kontrolní součet neexistuje

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zásada ochrany před únikem informací je 75%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:

  - Regulární výraz Regex_usa_bank_account_number najde obsah, který odpovídá vzoru

  - Najde se klíčové slovo z Keyword_usa_Bank_Account.

    Například následující ukázka by aktivovala zásady **bankovního účtu USA** : kontrola účtu 78344011

Další informace o tom, co je potřeba pro zjištění **čísla bankovního účtu US** pro váš obsah, najdete v tomto článku v následující části: [co citlivé typy informací hledají číslo bankovního účtu USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .
  
Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  