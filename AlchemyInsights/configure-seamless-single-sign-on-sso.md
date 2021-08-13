---
title: Konfigurace bezproblémového jednotného přihlašování (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966030"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurace bezproblémového jednotného přihlašování (SSO)

**Konfigurace aplikací**

1. Hodnoty byste měli získat od dodavatele aplikace. Hodnoty můžete zadat ručně nebo nahrát soubor metadat a extrahovat tak hodnotu polí.
2. Mnoho aplikací už je předkonfigurovaných pro práci s Azure AD. Tyto aplikace jsou uvedené v galerii aplikací, které můžete procházet, když přidáte aplikaci do tenanta Azure AD. Série [rychlých startů](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vás provede celým procesem.
3. Pokud chcete vytvořit aplikaci, která není galerie, můžete kliknout na **+ tlačítko** Vytvořit vlastní aplikaci a dát aplikaci název.
    - Ve výchozím nastavení  vybere možnost Integrovat jakoukoli jinou aplikaci, kterou v galerii nenajdete, což je správná možnost pro aplikace mimo galerii.
    - Jakmile po **uvedení** názvu aplikace na tlačítko Vytvořit, vytvoří se nová aplikace bez Enterprise galerie.
    - Potom můžete přejít na **jednotné** přihlašování  v části Správa této aplikace a uvidíte různé techniky implementace této aplikace ve vašem prostředí.

**Konfigurace bezproblémového jednotného přihlašování pro konkrétní aplikaci**

U aplikací v galerii najdete podrobné podrobné pokyny. Pokud chcete získat přístup k krokům, můžete procházet seznam všech kurzů konfigurace aplikací v kurzech pro konfiguraci aplikací [SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurace jednotného přihlašování založeného na protokolu SAML**

1. [Rychlý start: Nastavení jednotného přihlašování (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)založeného na protokolu SAML pro aplikaci v tenantovi Azure Active Directory (Azure AD).
2. Další informace o možnosti jednotného přihlašování založené na protokolu SAML najdete v tématu Principy jednotného přihlašování založeného na [samlu.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Další informace o žádostech o ověření SAML 2.0 a odpovědích, které Azure Active Directory (Azure AD) podporuje pro jednotné Sign-On přihlašování (SSO), najdete v tématu Jednotné přihlašování [Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Informace o tom, jak vytvořit a nakonfigurovat jednotné přihlašování založené na protokolu SAML (SSO) pro vaši aplikaci v Azure Active Directory (Azure AD) pomocí rozhraní Microsoft Graph [API,](https://docs.microsoft.com/graph/application-saml-sso-configure-api)najdete v tématu Konfigurace jednotného přihlašování založeného na protokolu SAML pro vaši aplikaci pomocí rozhraní Microsoft Graph API .
5. Informace o tom, jak Azure AD používá protokol SAML, najdete v článku Jak [Microsoft identity platform používá protokol SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfigurace tokenů a deklarací identity**

1. [Postupy: Přizpůsobení deklarací vydaných v tokenu SAML pro podnikové aplikace](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Informace o konfiguraci deklarací identity pomocí PowerShellu najdete v tématu Postup: Přizpůsobení deklarací identity vydávané v tokenech pro konkrétní aplikaci v [tenantovi (Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Informace o konfiguraci nepovinných deklarací identity najdete v tématu [Postup: Poskytnutí volitelných deklarací do aplikace](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Informace o tom, jak používat atributy rozšíření schématu adresáře pro posílání uživatelských dat do aplikací v deklaracích tokenů, najdete v tématu Použití atributů rozšíření [schématu adresáře v deklaracích identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Informace o konfiguraci životnosti tokenů najdete v tématu Konfigurace [životnosti tokenů v Microsoft identity platform (preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurace zásad životnosti tokenů (preview)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – V tomto článku procházíme běžným scénářem zásad, který vám může pomoct zavést nová pravidla pro životnost tokenů. V příkladu se dozvíte, jak vytvořit zásadu, která vyžaduje, aby uživatelé ve webové aplikaci ověřovat častěji.

**Poradce při potížích s konfigurací jednotného přihlašování**

- Časté otázky týkající se Azure Active Directory bezproblémového jednotného přihlašování Sign-On (Bezproblémové jednotné přihlašování) najdete v tématu Azure Active Directory Bezproblémové jednotné [přihlašování: Časté otázky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informace o běžných problémech týkajících se bezproblémového jednotného přihlašování Azure Active Directory (Azure AD Sign-On) najdete v tématu Řešení potíží Azure Active Directory jednotného [přihlašování](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
