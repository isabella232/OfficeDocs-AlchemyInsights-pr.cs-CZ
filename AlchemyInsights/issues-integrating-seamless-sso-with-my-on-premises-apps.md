---
title: Problémy s integrací bezproblémového jednotného přihlašování s místními aplikacemi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868650"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problémy s integrací bezproblémového jednotného přihlašování s místními aplikacemi

Pokud chcete řešit problémy s integrací bezproblémového jednotného přihlašování s místními aplikacemi, postupujte takto:

**Doporučené kroky**

1. Pokud chcete nakonfigurovat **místní aplikaci** pro **jednotné přihlašování prostřednictvím proxy serveru**, podívejte se na článek [trezor hesel pro jednotné přihlašování s aplikací proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Řešení problémů se službou proxy aplikací**: Doporučujeme začít s kontrolou toku řešení potíží, což je [problém s konektorem ladění aplikace proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)a zjistit, jestli jsou připojovací konektory aplikace proxy správně nakonfigurované. Pokud pořád máte potíže s připojením k aplikaci, postupujte podle kroků pro řešení potíží v tématu [ladění aplikací proxy aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). [Problémy CORS můžete identifikovat](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomocí následujících ladicích nástrojů prohlížeče:
    1. Spusťte prohlížeč a přejděte do webové aplikace.
    1. Stisknutím klávesy **F12** Zobrazte ladicí konzoli.
    1. Zkuste transakci zopakovat a zkontrolujte zprávu konzoly. Porušení CORS vyvolá chybu konzoly o původu.
    1. Některé problémy CORS nejdou vyřešit, třeba když váš aplikace přesměrovává na login.microsoftonline.com, a platnost tokenu přístupu vyprší. Volání CORS potom selže. Alternativním řešením pro tento scénář je prodloužit životnost accessového tokenu, aby nedocházelo k jeho vypršení během relace uživatele. Další informace o tom, jak postupovat, najdete [v článku Konfigurace životnosti tokenů v Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Doporučené dokumenty**

- [Jak nakonfigurovat jednotné přihlašování na aplikaci proxy aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Jednotné přihlašování pomocí protokolu SAML pro místní aplikace s proxy serverem aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Pochopení a řešení problémů s proxy aplikacemi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Poradce při potížích s omezením konfigurace delegování pro proxy server aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)