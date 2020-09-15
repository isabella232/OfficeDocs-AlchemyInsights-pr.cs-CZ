---
title: Antispam – 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717318"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Řešení problémů s doručováním e-mailů pro kód chyby 5.7.23

Ověřte záznam služby SPF DNS pro vaši doménu u veřejně dostupné kontroly záznamů SPF nebo DNS na webu.

Ověřte, že odchozí zpráva nebyla označena jako spam Microsoftu a směrována přes [vysoce rizikový fond](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Zprávy ve vysokém fondu pro doručování rizika neprojde kontroly SPF, a proto je cílová e-mailová organizace nepřijme.

Pokud potíže potrvají, obraťte se na správce hostitele pošty, na který se pokoušíte odeslat e-mail. Poznamenejte si podrobnou externí chybu, která je k dispozici ve zprávě o vrácení. Podporu Microsoftu nepůjde dále podporovat.
