---
title: Obdrželi vaši uživatelé škodlivý e-mail
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326653"
---
# <a name="did-your-users-receive-malicious-email"></a>Obdrželi vaši uživatelé škodlivý e-mail?

Škodlivý e-mail teď můžete microsoftu nahlásit pomocí [příspěvků na Microsoft 365 Defender portálu.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Zprávy odeslané v odeslání správce se [proskenuje](https://security.microsoft.com/reportsubmission?viewid=admin) a v podrobném plovoucím panelu se zobrazí následující výsledky:

- Pokud v době doručení došlo k chybě při ověřování e-mailu odesílatele.
- Informace o všech přístupech zásad, které mohly ovlivnit nebo přepsat vynesení zprávy.
- Aktuální výsledky detonace se dozvíte, jestli adresy URL nebo soubory obsažené ve zprávě byly škodlivé nebo ne.
- Zpětná vazba od graders

Pokud bylo nalezeno přepsání, mělo by se znovu prohledat během několika minut. Pokud v ověřování e-mailu nebyl problém nebo pokud se doručení neovlivňuje přepsáním, může zpětná vazba od graders trvat až jeden den.

Pokud nesouhlasíte s konečným verdiktem zprávy, adresy URL nebo souboru (blokované a nezablokované), odešlete zprávu znovu po dni, kdy chcete zprávu znovu prohledat. Pravděpodobnost, že se po odeslání zprávy znovu změní, je vysoká.

Mezitím můžete ze složky Doručená pošta uživatelů odebrat škodlivé e-maily podle pokynů v [tomto článku.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Zákazníci s Microsoft Defenderem pro Office 365 mohou:
  - Vyhledání a odstranění podezřelých [e-mailů pomocí](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered) Průzkumníka hrozeb
  - [Blokování Sejf k nebezpečné](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) adrese URL pomocí odkazů
  - Sledování uživatelů, kteří klikli na škodlivé adresy URL a přistupovali k nim: [Zobrazení adresy URL útoku phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)a kliknutí na vynesená data  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Ruční [spuštění automatizovaného vyšetřování](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Před škodlivými soubory a adresami URL můžete také chránit podle pokynů v tématu Ochrana před škodlivými [adresami URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)a soubory .
