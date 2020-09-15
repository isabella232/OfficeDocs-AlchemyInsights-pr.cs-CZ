---
title: Pravidlo ochrany před únikem čísla kreditní karty nefunguje
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679434"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Potíže s DLP s čísly kreditních karet

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Potíže s DLP s čísly kreditních karet**

Máte potíže s **zabráněním ztrátových dat (DLP)** , které nefungují u obsahu obsahujícího **číslo kreditní karty** v O365? Pokud ano, ujistěte se, že obsah obsahuje potřebné informace pro aktivaci zásady ochrany před únikem informací při vyhodnocování. Například pro **zásady platební karty** , které jsou nakonfigurovány s úrovní spolehlivosti 85%, jsou vyhodnoceny následující vyhodnocení a musí být rozpoznáno, aby pravidlo aktivovalo:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, které je možné formátovat nebo Neformátovat (dddddddddddddddd) a které musí projít testem Luhn.

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Velmi složité a robustní vzorky, které zjišťují karty všech hlavních značek po celém světě, včetně VISA, MasterCard, karty Discover, JCB, American Express, dárkových poukazů a Diner karet.

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ano, kontrolní součet Luhn

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Zásada ochrany před únikem informací je 85%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:

  - Funkce Func_credit_card najde obsah, který odpovídá vzoru.

  - Je to pravda:

  - Najde se klíčové slovo z Keyword_cc_verification.

  - Najde se klíčové slovo z Keyword_cc_name

  - Funkce Func_expiration_date najde datum ve správném formátu data.

  - Provedená kontrolní součty

    Například následující ukázka by mohla vyvolat zásadu pro nastavení čísel kreditní karty pro DLP:

  - Visa: 4485 3647 3952 7352
  
  - Platnost vyprší: 2/2009

Další informace o tom, co je potřeba pro zjištění **čísla kreditní karty** pro váš obsah, najdete v tomto článku v této části: [co citlivé typy informací vyhledají pro číslo kreditní karty #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  