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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821404"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Řešení problémů s doručováním e-mailů s kódem chyby 5.7.23

Ověřte záznam DNS SPF pro vaši doménu u veřejně dostupné kontroly záznamů SPF nebo DNS na webu.

Ověřte, že odchozí zpráva nebyla společností Microsoft identifikována jako spam a směrována prostřednictvím fondu pro doručování s vysokým [rizikem.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Zprávy ve fondu pro doručování s vysokým rizikem neprojdou kontrolami SPF, a proto nebudou akceptovány cílovou e-mailovou organizací.

Pokud problém potrvá, budete možná muset kontaktovat správce hostitele pošty, kterému se pokoušíte poslat e-mail. Poznamenejte si podrobnou externí chybu dostupnou ve zprávě o opuštění. Podpora Microsoftu nemusí být schopná dále pomáhat.
