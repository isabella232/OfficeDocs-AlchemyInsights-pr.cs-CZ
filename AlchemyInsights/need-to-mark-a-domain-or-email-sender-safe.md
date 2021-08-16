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
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025603"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?

- Použití seznamů **bezpečných odesílatelů se nedoporučuje,** protože se ve vaší organizaci otevírá útoky spamu, phish a falšování falšování.
- Pokud ale existuje obchodní požadavek, doporučujeme k tomu **[použít Flow mailových](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pravidel.  Naše pokyny zajistí ověření odesílatele (ověření, že se doména odesílání neschová). **Poznámka:** Nedoporučujeme spravovat falešná pozitiva pomocí seznamů bezpečných odesílatelů, protože výjimky z filtrování spamu mohou otevřít vaši organizaci kvůli útokům zabezpečení. Pokud vaši uživatel(é) dostávají zprávy nesprávně označené jako spam nebo nevyžádané e-maily, nahlásit zprávy a **[soubory microsoftu](https://protection.office.com/reportsubmission)**.
- Sejf Odesílatelům v Outlook, seznamu povolených odesílatelů nebo seznamu  povolených domén v zásadách ochrany proti spamu je třeba se vyhnout, protože odesílatelé obcházejí všechny spamy, falšování identity a phish protection a ověřování odesílatele (SPF, DKIM, DMARC). Tato metoda se nejlépe používá jenom pro dočasné testování.
- Ověření, že se některému **[e-mailu](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** nepomáhá hodnocení Antispamu, můžete provést kontrolou záhlaví zprávy X-Forefront-Antispam-Report (SFV:SFE, SFV:SKA, SFV:SKN), viz Záhlaví spamu .
- Vzhledem k tomu, že Microsoft chce ve výchozím [nastavení](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)udržovat naše zákazníky v bezpečí , některé přepsání tenanta se u malwaru a útoku phishing s vysokou spolehlivostí neuchytá. K těmto přepsáním patří: o Seznamy povolených odesílatelů nebo povolené seznamy domén (zásady ochrany proti spamu) o Outlook Sejf Odesílatelé o Seznam povolených ip adres (filtrování připojení) 
- Jediným přepsáním, které umožňuje, aby se phishingová zpráva s vysokou spolehlivostí vyhnula filtrování, Exchange pravidla toku pošty (označované také jako pravidla přenosu). Pokud chcete pomocí pravidel toku pošty obejít filtrování, podívejte se na informace v tématu Použití pravidel toku pošty k nastavení úrovně spolehlivosti spamu **[(SCL) ve zprávách](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.