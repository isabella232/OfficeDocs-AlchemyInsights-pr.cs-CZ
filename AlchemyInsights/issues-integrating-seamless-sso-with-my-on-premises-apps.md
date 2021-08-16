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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028285"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problémy s integrací bezproblémového jednotného přihlašování s místními aplikacemi

Pokud chcete vyřešit problémy s integrací bezproblémového jednotného přihlašování s místními aplikacemi, proveďte toto:

**Doporučené kroky**

1. Informace o konfiguraci **místní aplikace** pro jednotné přihlašování prostřednictvím proxy serveru aplikace **najdete** v tématu Trezor hesel pro jednotné přihlašování pomocí [Proxy aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Řešení problémů s proxy serverem** aplikace: Doporučujeme, abyste začali s kontrolami toku řešení potíží, ladění problémů s konektorem [Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)aplikací, abyste zjistili, jestli jsou konektory Proxy aplikací správně nakonfigurované. Pokud máte pořád problémy s připojením k aplikaci, postupujte podle pokynů pro řešení potíží s aplikací Proxy aplikací pro [ladění.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Problémy s [CORS můžete identifikovat](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomocí následujících nástrojů pro ladění prohlížeče:
    1. Spusťte prohlížeč a přejděte na webovou aplikaci.
    1. Stisknutím **klávesy F12** vytáhněte konzolu ladění.
    1. Zkuste transakci reprodukovat a zkontrolujte zprávu konzoly. Porušení CORS vytváří chybu konzoly týkající se původu.
    1. Některé problémy se službou CORS se neřeší, například když vaše aplikace přesměruje na login.microsoftonline.com k ověření a vyprší platnost přístupového tokenu. Volání CORS pak selže. Alternativním řešením tohoto scénáře je prodloužení životnosti přístupového tokenu, aby se zabránilo vypršení platnosti během relace uživatele. Další informace o tom, jak to udělat, najdete v tématu Konfigurace [životnosti tokenů](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)v Microsoft identity platform .

**Doporučené dokumenty**

- [Konfigurace jednotného přihlašování k aplikaci Proxy aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Jednotné přihlašování SAML pro místní aplikace pomocí Proxy aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Principy a řešení Azure Active Directory problémů s cors proxy aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Poradce při potížích s omezenými konfiguracemi delegování protokolu Kerberos pro proxy aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)