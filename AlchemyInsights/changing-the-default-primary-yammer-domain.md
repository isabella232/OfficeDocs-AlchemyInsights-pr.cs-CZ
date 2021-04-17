---
title: Změna výchozí domény Yammeru
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817947"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Změna výchozí/primární domény Yammeru

URL adresa Yammeru obsahuje aktuální název primární domény pro vaši síť Yammeru. Název domény se nemusí shodovat s názvem primární domény nastaveným v Office 365 nebo v Azure AD. Chování se mění v závislosti na počtu vlastních domén přidaných do tenanta a na tom, jestli je Yammer v podporované konfiguraci (1 tenant na 1 síť, nebo 1:1). K dispozici je dokumentace k [doménám Yammeru a Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Nejčastějším důvodem, proč vidíte nesprávnou doménu, je více sítí Yammeru, které je potřeba konsolidovat. Prvním a důležitým krokem je [konsolidace na jedinou síť](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) prostřednictvím nástroje na migraci sítě. To je potřeba dokončit, než budete nastavovat svou primární doménu.

**Žádné vlastní domény**

U nových tenantů se pro Yammer použije výchozí doména (např. fabrikam.onmicrosoft.com) tenanta. Primární doména je nastavená na yammer.com/fabrikam.onmicrosoft.com.

**Jedna vlastní doména**

Yammer automaticky vybere vlastní doménu (např. fabrikam.com) tenanta a nastaví ji jako primární doménu Yammeru. Je nastavená na yammer.com/fabrikam.com. Tuto změnu provádí služba synchronizace domén a může trvat až 24 hodin, než se projeví.

**Více vlastních domén**

Yammeru může mít doménu, která se od výchozí domény tenanta liší. Když existuje víc vlastních domén, Yammer se nebude pokoušet hádat, která z dostupných domén je ta správná. Bude potřeba, abyste požádali o změnu názvu primární domény na vámi vybranou doménu.

**Další informace o řešení potíží**

V některých případech se mohly domény přesunout mezi tenanty a službu synchronizace domén se nemuselo povést úspěšně spustit. Kromě nesprávné primární domény můžete mít potíže s přihlášením nebo jiné problémy. Když to budete chtít vyřešit, možná bude potřeba domény přesunout na správnou síť s pomocí podpory Microsoftu. Taková situace vyžaduje přímou asistenci a může nějakou dobu trvat, než se vyřeší. Zvláště pak tehdy, když je seznam domén opravdu dlouhý. Požádejte o asistenci s řešením podobných potíží.

Až budete spolupracovat se zástupcem podpory, ověří si, že je doména ověřená u tenanta, kterého spravujete vy. Pokud máte domény přidané k tenantovi, ale neověřené prostřednictvím DNS, možná bude kvůli ověření potřeba dodat další informace. Pokud chcete proces urychlit, ujistěte se, že jsou domény ověřené prostřednictvím DNS.
