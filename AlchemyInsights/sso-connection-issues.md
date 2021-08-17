---
title: Problémy s připojením jednotného přihlašování
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084339"
---
# <a name="sso-connection-issues"></a>Problémy s připojením jednotného přihlašování

1. Postupujte podle [rychlého startu: Konfigurace vlastností pro průvodce aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) pro konfiguraci aplikace.
2. V závislosti na [](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) aplikaci a možnosti jednotného přihlašování, které jste zvolili, postupujte podle následujících pokynů:
    - Informace o konfiguraci místní aplikace **pro** jednotné přihlašování založené na protokolu **SAML** najdete v tématu Jednotné přihlašování SAML pro místní aplikace pomocí [Proxy aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Informace o **konfiguraci cloudové aplikace pro** jednotné přihlašování založené na heslech najdete v tématu Konfigurace jednotného přihlašování pomocí  [hesla.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Informace o konfiguraci **místní aplikace** pro jednotné přihlašování prostřednictvím proxy serveru aplikace **najdete** v tématu Trezor hesel pro jednotné přihlašování pomocí [Proxy aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Řešení problémů s proxy aplikací**: Doporučujeme začít s kontrolami toku řešení potíží, problémů s [konektorem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)Proxy aplikací pro ladění , abyste zjistili, jestli jsou konektory Proxy aplikací správně nakonfigurované. Pokud máte pořád potíže s připojením k aplikaci, postupujte podle pokynů k řešení potíží s aplikací Proxy aplikací pro [ladění.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Problémy s [CORS můžete identifikovat](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomocí nástrojů pro ladění prohlížeče:
    - Spusťte prohlížeč a přejděte na webovou aplikaci.
    - Stisknutím **klávesy F12** vytáhněte konzolu ladění.
    - Zkuste transakci reprodukovat a zkontrolujte zprávu konzoly. Porušení CORS vytváří chybu konzoly týkající se původu.
    - Některé problémy se službou CORS se neřeší, například když vaše aplikace přesměruje login.microsoft.com ověřování a vyprší platnost přístupového tokenu. Volání CORS pak selže. Alternativním řešením tohoto scénáře je prodloužení životnosti přístupového tokenu, aby se zabránilo vypršení platnosti během relace uživatele. Další informace o tom, jak to udělat, najdete v tématu Konfigurace [životnosti tokenů](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)v Microsoft identity platform .
4. **Řešení potíží s** jednotným přihlašováním založeným na protokolu [SAML:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)Doporučujeme zkontrolovat problémy s přihlášením k aplikacím nakonfigurovaným pomocí jednotného přihlašování založeného na protokolu SAML a najít řešení problémů, se kterými se s největší pravděpodobností setkáte.
5. **Řešení potíží s** jednotným přihlašováním založeným na heslech : Doporučujeme zkontrolovat Poradce při potížích s jednotným přihlašováním založeným na heslech v [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)a najít řešení problémů, se kterými se s největší pravděpodobností setkáte.
6. Informace o problémech s připojením při používání vpn najdete v článku Jak používat jednotné přihlašování [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)přes VPN a Wi-Fi připojení.
