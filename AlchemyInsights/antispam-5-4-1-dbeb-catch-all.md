---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821440"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Řešení problémů s doručováním kódu chyby 550 5.4.1 Přístup k přenosu byl odepřen

K tomuto problému dochází [při kontrole,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) jestli je platná e-mailová adresa, aby se při zadávání do sítě Microsoft zabránilo návratu zpět. Vyzkoušejte následující postup:

1. Zjistěte, jestli je problém specifický pro celou doménu nebo jednu e-mailovou adresu:
    - Celá doména: Někdy je potřeba doménu synchronizovat. zkuste [nastavit doménu na Interní a potom zpátky na Autoritativní](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna e-mailová adresa: Někdy je potřeba adresu synchronizovat. může pomoct změna adresy proxy serveru smtp a jeho zpětná změna.
2. Zjistěte, jestli je problém specifický pro skupinu nebo veřejnou složku. U některých typů objektů může být potřeba objekty vytvořit ručně ve službě Azure Active Directory.

Pokud potřebujete další pomoc, otevřete lístek podpory a zadejte rozsah problému (včetně typu objektu, na který odesíláte), abychom vám mohli pomoct lépe.