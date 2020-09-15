---
title: Pravidlo ochrany před únikem pro SSN nefunguje
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679362"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problémy s DLP pomocí rodného čísla

**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).

**Problémy s DLP v SSNs**

Máte problémy s funkcí ochrany před únikem informací **(DLP)** , která nefunguje u **Social Security Number (SSN)** obsahu obsahujícího důvěrné informace v Microsoft 365? Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co vypadá zásada ochrany před únikem informací. 
  
Například zásady SSN, které jsou nakonfigurovány s úrovní spolehlivosti 85%, jsou vyhodnoceny a musí být detekovány, aby se pravidlo aktivovalo:
  
- **[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, která mohou být ve formátu, který není naformátován

- **[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Čtyři funkce hledejte SSNs ve čtyřech různých vzorcích:

  - Func_ssn najde SSNs 2011 s tučným formátováním, které je formátované pomocí pomlček nebo mezer (DDD-DD-dddd nebo DDD DD dddd).

  - Func_unformatted_ssn najde SSNs 2011 s neformátovaným silným formátováním (ddddddddd), které není formátované.

  - Func_randomized_formatted_ssn najde post-2011 SSNs, které jsou formátované pomocí pomlček nebo mezer (DDD-DD-dddd nebo DDD DD dddd).

  - Func_randomized_unformatted_ssn najde post-2011 SSNs, které nejsou formátované jako devět číslic za sebou (ddddddddd).

- **[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, kontrolní součet neexistuje

- **[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Zásada ochrany před únikem informací je 85%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:

  - [Funkce Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) najde obsah, který odpovídá vzoru.

  - Najde se klíčové slovo z [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Mezi příklady klíčových slov patří:  *sociální zabezpečení, sociálního zabezpečení #, SOC s, SSN*  . Například následující ukázka by mohla vyvolat zásadu ochrany před DLP: **SSN: 489-36-8350**
  
Další informace o tom, co je potřeba pro SSNs pro váš obsah, najdete v tomto článku v následující části: [co citlivé typy informací budou hledat pro SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) .
  
Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  