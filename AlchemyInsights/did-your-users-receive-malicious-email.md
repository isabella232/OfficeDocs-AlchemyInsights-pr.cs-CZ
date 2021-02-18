---
title: Obdrželi vaši uživatelé škodlivý e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291785"
---
# <a name="did-your-users-receive-malicious-email"></a>Obdrželi vaši uživatelé škodlivý e-mail?

- Teď můžete škodlivý e-mail nahlásit Microsoftu pomocí sestavy od správce v Centru zabezpečení a [dodržování předpisů & dodržování předpisů.](https://sip.protection.office.com/reportsubmission)

Zprávy odeslané v [odeslání](https://sip.protection.office.com/reportsubmission) správcem se skenovány a v podrobnostech se zobrazí **následující** výsledky:

- Pokud v době doručení došlo k chybě v ověření e-mailu odesílatele.
- Informace o přístupech k zásadám, které mohly ovlivnit nebo přepsaly hlavní název zprávy.
- Ve výsledcích aktuální detonace se dozvíte, jestli jsou adresy URL nebo soubory obsažené ve zprávě škodlivé nebo ne.
- Zpětná vazba od známkovatelů

Pokud se soubor přepíše, měl by se znovu zobrazit během několika minut. Pokud při ověřování e-mailu nebyl problém nebo pokud doručení nebylo ovlivněno přepsáním, může zpětnou vazbu od graders trvat až jeden den.

Pokud nesouhlasíte s konečným hodnocením zprávy, adresy URL nebo souboru (blokované a nezablokované), odešlete zprávu znovu po dni na remeš. Po odeslání zprávy se pravděpodobnost toho, že se hodnocení opět změní, je vysoká.

Mezitím můžete podle pokynů v tomto článku odebrat škodlivé e-maily ze složky Doručená [pošta uživatele.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Zákazníci, kteří mají Microsoft Defender pro Office 365, mohou:
    - Vyhledání [a odstranění podezřelého e-mailu pomocí Průzkumníka hrozeb](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [Blokování přístupu k škodlivé](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) adrese URL pomocí bezpečných odkazů
    - Sledování uživatelů, kteří klikli na škodlivé adresy URL a přistupovali k nim: Zobrazte [si adresu URL útoku phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)a klikněte na přehled dat  &  [Get-UrlTrace.](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - Ruční [spuštění automatického vyšetřování](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Můžete se také chránit před škodlivými soubory a adresami URL podle pokynů v článku Ochrana před škodlivými adresami URL a [soubory.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)