---
title: Pravidlo DLP pro číslo platební karty nefunguje
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005083"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problémy s DLP s čísly kreditních karet

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP s čísly kreditních karet**

Máte problémy s prevencí ztráty dat **(DLP)**  nefunguje pro obsah obsahující číslo platební karty při použití typu citlivých informací DLP v O365? Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace k aktivaci zásady ochrany před únikem informací při jejich vyhodnocení. Například u zásad platební karty nakonfigurovaných s úrovní spolehlivosti 85 % se vyhodnocují následující položky **a** musí být detekovány, aby pravidlo bylo možné aktivovat:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, které je možné formátovat nebo neformátovat (ddddddddddd) a musí projít luhnovou zkouškou.

- **[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Velmi složitý a robustní vzor, který detekuje karty od všech hlavních značek po celém světě, včetně karet Visa, MasterCard, Discover Card, JCB, American Express, dárkových karet a přání hosta.

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ano, kontrolní součet Luhn

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Zásada ochrany před únikem informací je z 85 % přesvědčená, že tento typ citlivých informací zjistila, pokud v blízkosti 300 znaků:

  - Funkce Func_credit_card najde obsah, který odpovídá vzoru.

  - Platí jedna z těchto podmínek:

  - Klíčové slovo z Keyword_cc_verification nalezené.

  - Klíčové slovo z Keyword_cc_name nalezené

  - Funkce Func_expiration_date najde datum ve správném formátu data.

  - Kontrolní součet projde

    Například následující ukázka by se spouštěl pro zásady číslování platební karty DLP:

  - Visa: 4485 3647 3952 7352
  
  - Vyprší: 2.2.2009

Další informace o tom,  co je potřeba pro zjištění čísla platební karty pro váš obsah, najdete v následující části v tomto článku: Co vypadají typy citlivých informací pro platební [kartu#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Informace o tom, co je potřeba pro jiné typy informací, najdete v následujícím článku s použitím jiného typu citlivých [informací:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Co tyto typy citlivých informací vypadají
  