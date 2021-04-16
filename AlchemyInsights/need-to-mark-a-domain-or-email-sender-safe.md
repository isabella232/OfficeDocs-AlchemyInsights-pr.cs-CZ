---
title: Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792125"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?

- Použití seznamů **bezpečných odesílatelů se nedoporučuje,** protože se ve vaší organizaci otevírá útoky spamu, phish a falšování falšování.
- Pokud ale existuje obchodní požadavek, doporučujeme **k** tomu použít pravidla **[toku](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pošty. Naše pokyny zajistí ověření odesílatele (ověření, že se doména odesílání neschová). **Poznámka:** Nedoporučujeme spravovat falešná pozitiva pomocí seznamů bezpečných odesílatelů, protože výjimky z filtrování spamu mohou otevřít vaši organizaci kvůli útokům zabezpečení. Pokud vaši uživatel(é) dostávají zprávy nesprávně označené jako spam nebo nevyžádané e-maily, nahlásit zprávy a **[soubory microsoftu](https://protection.office.com/reportsubmission)**.
- Je třeba se vyhnout bezpečným odesílatelům v Outlooku, seznamu povolených odesílatelů nebo seznamu povolených domén v zásadách ochrany proti spamu, protože odesílatelé obcházejí veškerý spam, falšování identity a phish ochranu a ověřování odesílatele (SPF, DKIM, DMARC).  Tato metoda se nejlépe používá jenom pro dočasné testování.
