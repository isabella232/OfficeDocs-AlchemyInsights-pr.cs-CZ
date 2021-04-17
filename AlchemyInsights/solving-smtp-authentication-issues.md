---
title: Řešení problémů s ověřováním SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826408"
---
# <a name="solving-smtp-authentication-issues"></a>Řešení problémů s ověřováním SMTP

Pokud se při pokusu o odeslání e-mailu SMTP a ověření pomocí klienta nebo aplikace zobrazí chyby 5.7.57 nebo 5.7.3, měli byste zkontrolovat několik věcí:

- Ověřené odeslání SMTP může být ve vašem tenantovi zakázané nebo v poštovní schránce, kterou se pokoušíte použít (zkontrolujte obě nastavení). Další informace najdete v tématu Povolení nebo zakázání odesílání protokolu [SMTP ověřeného klienta](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Zkontrolujte, [jestli je pro vašeho tenanta](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) povolené výchozí nastavení zabezpečení Azure. Pokud je tato možnost povolená, ověřování SMTP pomocí základního ověřování (označované také jako starší verze, použije se uživatelské jméno a heslo).
