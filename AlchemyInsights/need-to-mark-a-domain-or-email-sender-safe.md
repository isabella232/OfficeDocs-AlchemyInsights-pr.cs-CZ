---
title: Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803238"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?

- Používání **seznamů bezpečných odesílatelů se nedoporučuje** , protože otevře vaši organizaci útoky spamu, phishingu a falšování identity.
- Pokud je ale požadován podnik, **doporučujeme použít pro** toto **[pravidlo toku pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Naše pokyny zajistí ověření odesílatele (ověřuje, jestli není zafalešnovaná doména). **Poznámka**: Nedoporučujeme správu falešných falešných zpráv pomocí seznamů bezpečných odesílatelů, protože výjimky pro filtrování spamu můžou vaši organizaci otevřít na útoky zabezpečení. Pokud vaše uživatelé neoznačili zprávy nesprávně označené jako spam nebo Nevyžádaná pošta, **[ohlaste jim zprávy a soubory Microsoftu](https://protection.office.com/reportsubmission)**.
- Bezpeční odesílatelé v Outlooku, seznamu povolených odesílatelů nebo seznam povolených domén v zásadách ochrany před nevyžádanou poštou **by měli být zabráněno** , protože odesílatelé vycházejí ze všech spamů, falešných zpráv a ochrany proti podvodné poště (SPF, DKIM, DMARC). Tento způsob je nejvhodnější pro dočasné testování.
