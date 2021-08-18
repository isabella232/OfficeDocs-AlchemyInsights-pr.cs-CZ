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
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319941"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?

- Použití seznamů **bezpečných odesílatelů se nedoporučuje,** protože se ve vaší organizaci otevírá útoky spamu, phish a falšování.
- Pokud ale existuje obchodní požadavek, doporučujeme **k** tomu použít **[Flow mailových](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pravidel. Naše pokyny zajišťují ověřování odesílatele (ověření, že se doména odesílání neschová. 
    **Poznámka:** Nedoporučujeme spravovat falešná pozitiva pomocí seznamů bezpečných odesílatelů, protože výjimky z filtrování spamu mohou otevřít vaši organizaci kvůli útokům zabezpečení. Pokud vaši uživatel(é) dostávají zprávy nesprávně označené jako spam nebo nevyžádaná pošta, nahlásit zprávy a **[soubory Microsoftu](https://protection.office.com/reportsubmission)**.
- Sejf Odesílatelům v Outlook, seznamu povolených odesílatelů nebo seznamu  povolených domén v zásadách ochrany proti spamu je třeba se vyhnout, protože odesílatelé obcházejí veškerý spam, falšování identity a phish ochranu a ověřování odesílatele (SPF, DKIM, DMARC). Tato metoda se nejlépe používá jenom pro dočasné testování.
- Ověření, že se některému **[e-mailu](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** nepomáhá hodnocení Antispamu, můžete provést kontrolou záhlaví zprávy X-Forefront-Antispam-Report (SFV:SFE, SFV:SKA, SFV:SKN), viz Záhlaví spamu .
- Vzhledem k tomu, že Microsoft chce ve výchozím [nastavení](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)udržovat naše zákazníky v bezpečí , některá přepsání tenanta se u malwaru a útoku phishing s vysokou spolehlivostí neuchytá. Mezi tato přepsání patří: o Seznamy povolených odesílatelů nebo seznamy povolených domén (zásady ochrany proti spamu) o Outlook Sejf Odesílatelé o Seznam povolených IP adres (filtrování připojení) 
- Jediným přepsáním, které umožňuje, aby se phishingová zpráva s vysokou spolehlivostí vyhnula filtrování, Exchange pravidla toku pošty (označované taky jako pravidla přenosu). Pokud chcete k obcházení filtrování použít pravidla toku pošty, podívejte se na informace v tématu Použití pravidel toku pošty k nastavení úrovně spolehlivosti spamu **[ve zprávách](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.