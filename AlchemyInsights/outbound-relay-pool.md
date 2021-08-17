---
title: Fond odchozích přenosů
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: d2f83b3afc4abf72a3e18bffe5ac9d6c940cc216916925338c18f0fb8a39948a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883124"
---
# <a name="outbound-relay-pool"></a>Fond odchozích přenosů

Microsoft v konfiguraci přenosu nebo přeposílání e-mailů prostřednictvím Microsoft 365. Zprávy v určitých situacích se přeposílá nebo přeposílá přes Microsoft 365 pomocí speciálního fondu přenosů. Zprávy odeslané pomocí fondu přenosů by mohly skončit ve složce nevyžádané pošty příjemce. Další informace najdete v tématu [Fondy odchozích doručení.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Abyste se vyhnuli scénáři použití fondu přenosů, ujistěte se, že přeposlané/předáné zprávy splňují jedno z následujících kritérií:

- Odchozí odesílatel je akceptována doména tenanta.
- Rozhraní SPF (Sender Policy Framework) projde, když se zpráva zobrazí Microsoft 365.
- DomainKeys Identified Mail (DKIM) v doméně odesílatele P2 projde, když se zpráva zobrazí Microsoft 365.
 
Zprávy, které splňují výše uvedená kritéria, se přes fond přenosu nesměruje.

Pokud je záznam MX pro vaši doménu namířil na server třetí strany nebo místního serveru, použijte vylepšené filtrování, abyste měli jistotu, že je ověření SPF správné pro příchozí e-maily a abyste se vyhnuli odesílání e-mailů prostřednictvím fondu přenosů.

**Jak můžeme zjistit, jestli nás ovlivňuje fond přenosů?**

Pokud vaše přeposlané nebo předáené e-maily používají jedno z výše uvedených kritérií, zprávy se přes fond přenosů nepřesílat nebudou. Pokud se ale zpráva odesílá prostřednictvím fondu přenosů, ip adresa odchozího serveru je v oblasti 40.95.0.0/16 a název odchozího serveru obsahuje **rly** v názvu.

