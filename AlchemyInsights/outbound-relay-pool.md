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
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041579"
---
# <a name="outbound-relay-pool"></a>Fond odchozích přenosů

Microsoft v konfiguraci přenosu nebo přeposílání e-mailů prostřednictvím Microsoft 365. Zprávy v určitých situacích se přeposílá nebo přeposílá přes Microsoft 365 pomocí speciálního fondu přenosů. Zprávy odeslané pomocí fondu přenosů by mohly skončit ve složce nevyžádané pošty příjemce. Další informace najdete v tématu [Fondy odchozích doručení.](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Abyste se vyhnuli scénáři použití fondu přenosů, ujistěte se, že přeposlané/předáné zprávy splňují jedno z následujících kritérií:

- Odchozí odesílatel je akceptována doména tenanta.
- Rozhraní SPF (Sender Policy Framework) předá, když se zpráva zobrazí Microsoft 365.
- DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.
 
Zprávy, které splňují výše uvedená kritéria, se přes fond přenosu nesměruje.

Pokud záznam MX pro vaši doménu odkazuje na server třetí strany nebo místního serveru, použijte vylepšené filtrování, abyste měli jistotu, že je ověření SPF správné pro příchozí e-maily a abyste se vyhnuli posílání e-mailů prostřednictvím fondu přenosu.

**Jak můžeme zjistit, jestli nás ovlivňuje fond přenosů?**

Pokud vaše přeposlané nebo předáené e-maily používají jedno z výše uvedených kritérií, zprávy se přes fond přenosů nepřesílat nebudou. Pokud se ale zpráva odesílá prostřednictvím fondu přenosů, ip adresa odchozího serveru je v oblasti 40.95.0.0/16 a název odchozího serveru obsahuje **rly** v názvu.

