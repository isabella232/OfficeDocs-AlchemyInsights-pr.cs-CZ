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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932270"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Řešení problémů s doručováním kódu chyby 550 5.4.1 Přístup k přenosu byl odepřen

K tomuto problému dochází [při kontrole,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) jestli je platná e-mailová adresa, aby se při zadávání do sítě Microsoft zabránilo návratu zpět. Vyzkoušejte následující postup:

1. Zjistěte, jestli je problém specifický pro celou doménu nebo jednu e-mailovou adresu:
    - Celá doména: Někdy je potřeba doménu synchronizovat. zkuste [nastavit doménu na Interní a potom zpátky na Autoritativní](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna e-mailová adresa: Někdy je potřeba adresu synchronizovat. může pomoct změna adresy proxy serveru smtp a jeho zpětná změna.
2. Zjistěte, jestli je problém specifický pro skupinu nebo veřejnou složku. U některých typů objektů může být potřeba objekty vytvořit ručně v Azure Active Directory.

Pokud potřebujete další pomoc, otevřete lístek podpory a zadejte rozsah problému (včetně typu objektu, na který odesíláte), abychom vám mohli pomoct lépe.