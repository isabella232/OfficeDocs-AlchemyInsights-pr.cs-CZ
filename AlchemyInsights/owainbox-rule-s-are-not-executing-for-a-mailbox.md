---
title: 1332 OWA - Pravidla doručené pošty se neprovádí pro poštovní schránku
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576553"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravidlo složky Doručená pošta nefunguje podle očekávání

Ověřte v Outlooku na webu následující nastavení:

- Zprávu lze přesměrovat, přeposlat dál nebo automaticky odpovědět na základě pravidel doručené pošty pouze jednou. Pravidlo přesměrování (pravidlo doručené pošty nebo pravidlo toku pošty, označované také jako pravidlo přenosu) může do zprávy přidat maximálně deset příjemců předávání. Další informace naleznete v [tématu Journal, Transport a Inbox omezení pravidel](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravidla doručené pošty nefungují na alternativní poštovní schránky deníku. Další informace o alternativní poštovní schránce deníku naleznete [v tématu Alternativní ukládání poštovní schránky do deníku](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Tyto problémy naleznete v [tématu KB 2829319](https://support.microsoft.com/kb/2829319).

Pokud předchozí problémy neplatí, spusťte před eskalací problému na podporu microsoftu diagnostickou sestavu diagnostiky pravidel doručené pošty:

1. Otevřete poštovní schránku v Outlooku na webu a klikněte na <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Nastavení**  >  **Zobrazit všechna nastavení**  >  aplikace Outlook **Pošta**  >  **Pravidla**.

2. V dolní části stránky klikněte na **Pokud pravidla nefungují, klikněte sem a vygenerujte diagnostickou sestavu**.
