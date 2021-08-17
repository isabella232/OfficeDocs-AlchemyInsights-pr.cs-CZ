---
title: 1332 OWA – pravidla doručené pošty se pro poštovní schránku neschová.
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040895"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravidlo doručené pošty nefunguje podle očekávání.

Ověřte následující nastavení v Outlook na webu:

- Zprávu můžete přesměrovat, přeposlat nebo na kterou můžete na základě pravidel doručené pošty automaticky na základě pravidel doručené pošty jenom jednou. Pravidlo přesměrování (pravidlo doručené pošty nebo pravidlo toku pošty, označované také jako pravidlo přenosu) může do zprávy přidat maximálně deset příjemců přeposílání. Další informace najdete v článku Omezení pravidel [deníku, přenosu a doručené pošty](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravidla doručené pošty nefungují na alternativní poštovní schránce deníku. Další informace o alternativní poštovní schránce pro ukládání do deníku najdete v tématu [Alternativní poštovní schránka deníku](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Pokud chcete tyto problémy vyřešit, podívejte [se na článek KB 2829319](https://support.microsoft.com/kb/2829319).

Pokud se předchozí problémy nevztahují, spusťte před eskalátorem problému diagnostickou sestavu pravidel doručené pošty na podporu Microsoftu:

1. Otevřete poštovní schránku v Outlook na webu a klikněte na <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Nastavení**  >  **Zobrazit všechny Outlook Nastavení**  >  **Pošta**  >  **Pravidla**.

2. V dolní části stránky klikněte na Pokud vaše pravidla nefungují, klikněte sem a vygenerte **diagnostickou sestavu.**
