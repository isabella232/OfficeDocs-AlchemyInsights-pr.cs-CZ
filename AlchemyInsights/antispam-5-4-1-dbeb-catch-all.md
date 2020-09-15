---
title: AntiSpam 5.4.1 DBEB catch – vše
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717354"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Řešení problémů s doručováním kódu chyby 550 5.4.1 odepření přístupu

K tomuto problému dochází, když se [zkontroluje, jestli e-mailová adresa není platná pro zabránění bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) při vstupu do sítě Microsoftu. Vyzkoušejte toto:

1. Zjistěte, jestli je problém specifický pro celou doménu nebo jednu e-mailovou adresu:
    - Celá doména: doménu je někdy třeba synchronizovat. Zkuste [doménu nastavit jako interní a potom zpět na autoritativní](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jediná e-mailová adresa: někdy je třeba adresu synchronizovat. můžete změnit adresu proxy serveru SMTP a pak ji znovu změnit.
2. Zjistěte, jestli je problém specifický pro skupinu nebo veřejnou složku. U některých typů objektů je nutné, aby byly objekty ručně vytvořeny v Azure Active Directory.

Pokud potřebujete další pomoc, otevřete lístek podpory a zadejte obor problému (včetně typu objektu, na který posíláte), abychom vám mohli pomoct lépe.