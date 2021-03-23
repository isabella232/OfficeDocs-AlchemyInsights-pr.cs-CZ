---
title: Řešení potíží s protokoly OAuth 2.0 a OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035171"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Řešení potíží s protokoly OAuth 2.0 a OpenID Connect

Pokud chcete vyřešit problémy s OAuth 2.0 a OpenID Connect, proveďte následující doporučené kroky:

Podívejte se na následující články týkající se konfigurace a řešení potíží s protokoly OAuth 2.0 a OpenID Connect:

- Platforma identit Microsoftu a tok autorizačního kódu [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Tento článek popisuje, jak programovat přímo proti toku kódu **(PKCE)** v aplikaci pomocí libovolného jazyka.
- Platforma identit Microsoftu a tok přihlašovacích údajů klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Tento článek popisuje, jak naprogramovat přímo proti toku přihlašovacích údajů klienta ve vaší aplikaci. 
- Platforma identit Microsoftu a přihlašovací údaje pro heslo vlastníka prostředků [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – tento článek popisuje, jak programovat přímo proti toku **ROPC** ve vaší aplikaci.
    - Platforma identit Microsoftu podporuje jenom ROPC pro tenanty Azure AD, a ne pro osobní účty. To znamená, že musíte použít koncový bod specifický pro **tenanta https://login.microsoftonline.com/{TenantId_or_Name}) (** nebo koncový **bod** organizace.
    - Osobní účty, které jsou pozvaní do tenanta Azure AD, nesměvají používat ROPC.
    - Účty, které nemají hesla, se přes ROPC neschová. V tomto scénáři doporučujeme místo toho použít jiný tok pro vaši aplikaci.
    - Pokud se uživatelé potřebují [k přihlášení](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) k aplikaci přihlásit pomocí vícefaktorového ověřování, zablokují se.
    - Funkce ROPC není podporovaná ve [scénářích](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) federace hybridní identity (například Azure AD a ADFS používané k ověřování místních účtů). Pokud jsou uživatelé přesměrováni na celou stránku na místního poskytovatele identity, Služba Azure AD nemůže otestovat uživatelské jméno a heslo u tohoto poskytovatele identity. [Ověřování předávk ů](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) je ale podporované u ropcu.
    - Výjimkou ze scénáře federace hybridní identity by byla tato: Zásady zjišťování domovské oblasti s **vlastností AllowCloudPasswordValidation** nastavenou na **hodnotu PRAVDA** umožní tok ROPC fungovat federovaným uživatelům, když se místní heslo synchronizuje do cloudu. Další informace najdete v tématu [Povolení přímého ověřování ROPC federovaných uživatelů pro starší aplikace.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Platforma identit Microsoftu a OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – Tento článek popisuje, jak programovat přímo proti toku **OBO (on-behalf-of)** ve vaší aplikaci.
- [Platforma identit Microsoftu](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) a protokol OpenID Connect – tento článek ukazuje, jak implementovat protokol OpenID Connect nezávisle na jazyce, a popisuje, jak odesílat a přijímat zprávy HTTP bez použití open-source knihoven Microsoftu.

**Přístupové tokeny**

[Přístupové tokeny platformy Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) identity – Zjistěte, jak může rozhraní API ověřovat a používat deklarace identity uvnitř přístupového tokenu. Veškerá dokumentace v tomto článku, s výjimkou případů uvedených, platí jenom pro tokeny vydané pro rozhraní API, která jste zaregistrovali. Nevztahuje se na tokeny vydané pro rozhraní API vlastněné společností Microsoft a tyto tokeny se nedávají použít k ověření, jak bude platforma identit Microsoft vydávat tokeny pro rozhraní API, které vytvoříte.

**Konfigurace aplikace**

[Omezení a omezení identifikátoru URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url) pro přesměrování (adresa URL odpovědi) – zjistěte, jak nakonfigurovat identifikátor URI přesměrování (adresa URL odpovědi). Identifikátor URI přesměrování nebo adresa URL odpovědi je místo, kam autorizační server odešle uživatele, jakmile bude aplikace úspěšně autorizována a udělena autorizační kód nebo přístupový token. Autorizační server odešle kód nebo token identifikátoru URI přesměrování. proto je důležité, abyste v rámci procesu registrace aplikace zaregistroval správné umístění.

**Zřizování aplikací**

[Kurz: Vývoj a plánování](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) zřizování koncového bodu SCIM – tento článek popisuje, jak vytvořit koncový bod SCIM a integrovat se službou zřizování AAD.


