---
title: Antispam – 5,7,23
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
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932162"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Řešení problémů s doručováním e-mailů s kódem chyby 5.7.23

Ověřte záznam DNS SPF pro vaši doménu u veřejně dostupné kontroly záznamů SPF nebo DNS na webu.

Ověřte, že odchozí zpráva nebyla společností Microsoft identifikována jako spam a směrována prostřednictvím fondu pro doručování s vysokým [rizikem.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Zprávy ve fondu pro doručování s vysokým rizikem neprojdou kontrolami SPF, a proto nebudou akceptovány cílovou e-mailovou organizací.

Pokud problém potrvá, budete možná muset kontaktovat správce hostitele pošty, kterému se pokoušíte poslat e-mail. Poznamenejte si podrobnou externí chybu dostupnou ve zprávě o opuštění. Podpora Microsoftu nemusí být schopná dále pomáhat.
