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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935086"
---
# <a name="sso-connection-issues"></a>Problémy s připojením jednotného přihlašování

1. Postupujte podle [úvodní příručky: Konfigurace vlastností pro](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) průvodce aplikací pro konfiguraci aplikace.
2. Podle aplikace a [možnosti](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) jednotného přihlašování, kterou jste zvolili, postupujte podle odpovídajících pokynů níže:
    - Pokud chcete nakonfigurovat **místní** aplikaci pro jednotné přihlašování založené na **saml,** podívejte se na jednotné přihlašování SAML pro místní aplikace pomocí proxy [serveru aplikace.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Informace o **konfiguraci cloudové** **aplikace** pro jednotné přihlašování založené na heslech najdete v tématu Konfigurace jednotného přihlašování pomocí [hesla.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Pokud chcete nakonfigurovat **místní** aplikaci pro jednotné přihlašování prostřednictvím proxy serveru **aplikace,** podívejte se na trezor hesel pro jednotné přihlašování pomocí proxy [serveru aplikace.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Řešení problémů s proxy aplikací:** doporučujeme začít s revizemi toku pro řešení [potíží,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problémy s konektorem Proxy aplikace pro ladění, abyste zjistili, jestli jsou konektory proxy aplikace správně nakonfigurované. Pokud máte pořád problémy s připojením k aplikaci, postupujte podle pokynů pro řešení potíží v problémech s aplikací Proxy aplikací [pro ladění aplikací.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Problémy s [korsou můžete identifikovat pomocí](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) nástrojů pro ladění prohlížeče:
    - Spusťte prohlížeč a přejděte k webové aplikaci.
    - Stisknutím **klávesy F12** vytáhněte konzolu pro ladění.
    - Pokuste se transakci reprodukovat a zkontrolujte zprávu konzole. Porušení funkce CORS vytváří chybu konzole v přibližně počátcích.
    - Některé problémy s KORS není možné vyřešit, například když vaše aplikace přesměruje login.microsoft.com ověření a platnost přístupového tokenu vyprší. Poté selže volání funkce CORS. Řešením tohoto scénáře je prodloužení životnosti přístupového tokenu, aby se zabránilo vypršení platnosti během relace uživatele. Další informace o tom, jak to udělat, najdete v tématu Konfigurovatelné [životnosti tokenů na platformě identit Microsoftu.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **Řešení problémů jednotného** přihlašování založeného na serveru SAML: Doporučujeme zkontrolovat problémy s přihlášením k nakonfigurovaným aplikacím založeným na jednotném přihlašování na základě [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)abyste našli řešení problémů, se kterými se s největší pravděpodobností setkáte.
5. **Poradce při potížích s** jednotným přihlašováním založeným na heslech: Doporučujeme zkontrolovat v [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)řešení problémů s jednotným přihlašováním pomocí hesla a najít řešení problémů, se kterými se s největší pravděpodobností setkáte.
6. Problémy s připojením při používání VPN najdete v článku Jak používat jednotné přihlašování [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)přes VPN a Wi-Fi připojení.
