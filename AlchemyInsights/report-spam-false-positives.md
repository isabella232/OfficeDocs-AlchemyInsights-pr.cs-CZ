---
title: Chcete microsoftu nahlásit falešně pozitivní spam?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396608"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Označují se vám legitimní zprávy jako spam?

Je to frustrující, když legitimní e-mail skončí ve složce Nevyžádaná pošta nebo v karanténě. Zvažte tyto nejčastější důvody falešně pozitivních výsledků:

**Přepsání tenanta (nejběžnější)** To je plně v rámci vaší ovládacího prvku k nápravě.

Odešlete zprávu na Microsoft 365 Defender k analýze zásad a pravidel, které mají vliv. podrobnosti o opětovném prohledávání jsou k dispozici během několika minut.
Zkontrolujte nebo upravte zásady nebo pravidla podle příslušných předpisů. 

**Přepsání koncového uživatele (běžné)** To je plně v rámci vaší ovládacího prvku k nápravě. 

Odešlete zprávu na Microsoft 365 Defender k analýze zásad a pravidel, které mají vliv. podrobnosti o opětovném prohledávání jsou k dispozici během několika minut. 

Pokud byla zpráva zablokovaná, protože byla odeslána z adresy v seznamu blokovaných odesílatelů uživatele, záhlaví obsahují verdikt filtrování spamu "SFV:BLK".

**Ověřování e-mailem odesílatele** To je částečně v rámci vaší ovládacího prvku k nápravě.

Odešlete zprávu, abyste analyzovali chyby v ověřování e-mailu odesílatele v okamžiku doručení. výsledky jsou dostupné během jednoho dne. 

Pokud vlastníte odesílající infrastrukturu, zkontrolujte, jak ji zarovnat s SPF, DKIM a DMARC, abyste měli jistotu, že cílové e-mailové systémy důvěřují zprávám odeslaných z vaší domény. Případně kontaktujte odesílatele a požádejte o řešení jejich konfigurací DNS.

**Rozhodnutí o filtrování microsoftu** To je částečně v rámci vaší ovládacího prvku k nápravě.

Odešlete zprávu a nahlásit zprávu jako bezpečnou. výsledky vyhledávání jsou dostupné během jednoho dne. Seznam povolení a blokování tenanta použijte, když nesouhlasíte s filtrováním vynesených rozhodnutí v konkrétních situacích. Neměli byste ale trvale obcházet vynesení vynesení filtrování microsoftu. 

Další informace najdete tady:

- Povolte koncovým uživatelům odesílat zprávy do Microsoftu. Microsoft používá tato odeslání ke zlepšení účinnosti technologií ochrany e-mailu a zobrazí se v sestavách odeslání, které můžete použít jako indikaci aktualizace zásad. 

- Pokud se chcete podívat na krátké video o odesílání zpráv k analýze, podívejte se na téma Odesílání [zpráv pro analýzu](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Odeslání správce k odeslání podezření na spam, phish, adresy URL a soubory do Microsoftu](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Správa seznamu povolení a blokování tenanta](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Záhlaví nevyžádané pošty v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Ochrana proti odchozímu spamu v EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)