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
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929190"
---
# <a name="did-your-users-receive-malicious-email"></a>Obdrželi vaši uživatelé škodlivý e-mail?

- Škodlivý e-mail teď můžete microsoftu nahlásit pomocí příspěvku správce v [Centru & dodržování předpisů](https://sip.protection.office.com/reportsubmission).

Zprávy, které se posílají [v odeslání](https://sip.protection.office.com/reportsubmission) správce, se proskenuje a v plovoucím panelu podrobností se zobrazí **následující** výsledky:

- Pokud v době doručení došlo k chybě při ověřování e-mailu odesílatele.
- Informace o všech přístupech zásad, které mohly ovlivnit nebo přepsat vynesení zprávy.
- Aktuální výsledky detonace se dozvíte, jestli adresy URL nebo soubory obsažené ve zprávě byly škodlivé nebo ne.
- Zpětná vazba od graders

Pokud bylo nalezeno přepsání, mělo by se znovu prohledat během několika minut. Pokud v ověřování e-mailu nebyl žádný problém nebo pokud se doručení neovlivňuje přepsáním, může zpětná vazba od graders trvat až jeden den.

Pokud nesouhlasíte s konečným verdiktem zprávy, adresy URL nebo souboru (blokované a nezablokované), odešlete zprávu znovu po dni, kdy chcete zprávu znovu prohledat. Pravděpodobnost, že se po odeslání zprávy znovu změní, je vysoká.

Mezitím můžete ze složky Doručená pošta uživatelů odebrat škodlivé e-maily podle pokynů v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Zákazníci s Microsoft Defenderem pro Office 365 mohou:
    - Vyhledání a odstranění podezřelých [e-mailů pomocí](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered) Průzkumníka hrozeb
    - [Blokování Sejf škodlivé](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) adresy URL pomocí odkazů
    - sledování uživatelů, kteří klikli na škodlivé adresy URL a přistupovali k nim: Zobrazení adresy URL útoku phishing a kliknutí [na vynesená data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - ruční [spuštění automatizovaného vyšetřování](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Můžete také chránit před škodlivými soubory a adresami URL podle pokynů v tématu Ochrana před škodlivými [adresami URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)a soubory .