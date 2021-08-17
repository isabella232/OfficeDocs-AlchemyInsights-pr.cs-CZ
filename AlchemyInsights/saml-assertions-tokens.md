---
title: Kontrolní výrazy SAML (tokeny)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109233"
---
# <a name="saml-assertions-tokens"></a>Kontrolní výrazy SAML (tokeny)

1. Tokeny SAML (Security Assertions Markup Language) jsou xml reprezentace deklarací identity. Ve výchozím nastavení se tokeny SAML Windows Communication Foundation (WCF) ve scénářích federovaného zabezpečení vystaví tokeny. Další informace najdete v tématu [Tokeny SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)a deklarace identity .
2. Funkce Microsoft identity platform vysílá několik typů tokenů zabezpečení při zpracování každého toku ověřování. [Odkaz na deklarace tokenů SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) popisuje formát, vlastnosti zabezpečení a obsah tokenů SAML 2.0.
3. Postupujte podle pokynů v [tématu Konfigurovatelné životnosti tokenů v Microsoft identity platform,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) abyste pochopili, jak nakonfigurovat životnost tokenů.
4. Postupujte podle pokynů uvedených v [tomto článku,](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) abyste pochopili, jak nakonfigurovat šifrování tokenů Azure AD SAML.
5. V Azure AD můžete nastavit možnosti podepisování certifikátů a algoritmus podepisování certifikátů. Další informace najdete v článku [Rozšířené možnosti podepisování](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)certifikátů v tokenu SAML pro aplikace galerie v Azure Active Directory .
