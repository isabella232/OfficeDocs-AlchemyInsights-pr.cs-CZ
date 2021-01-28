---
title: Problémy s atributy a deklarace tokenů
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035852"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problémy s atributy a deklarace tokenů

**Aktualizace, konfigurace nebo odebrání deklarace tokenů**

1. Pomocí Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) můžete přizpůsobit typ deklarace identity pro claim role v tokenu pro odpověď, který dostanete po autorizaci aplikace.
2. Vývojáři aplikací mohou ve svých aplikacích Azure AD používat volitelné nároky k určení toho, jaké nároky chtějí mít v tokenech posílaných do své aplikace. Další informace najdete v článku [Poskytnutí nepovinných](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)nároků ve vaší aplikaci.
3. [Nakonfigurujte deklarace skupin pro aplikace pomocí Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Pokud používáte bezproblémové jednotné přihlašování ve vaší aplikaci, podívejte se na přizpůsobení nároků vydaných [v tokenu SAML pro podnikové aplikace.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mapování atributů deklarací**

1. Pokud chcete nakonfigurovat zásady mapování deklarací identity pomocí PowerShellu, podívejte se na stránku Přizpůsobení deklarací identity sílané do tokenů konkrétní aplikace v [tenantovi (Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atributy rozšíření schématu adresáře umožňují ukládat do Azure Active Directory další data v objektech uživatelů a jiných adresářových objektech, jako jsou skupiny, podrobnosti o tenantovi a objekty zabezpečení služby. K uplatnění nároku na nároky na aplikace lze použít pouze atributy rozšíření u uživatelských objektů. [Použití atributů rozšíření schématu adresáře v claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) popisuje, jak používat atributy rozšíření schématu adresáře pro odesílání uživatelských dat aplikacím v deklaracích tokenů.

Další informace o deklaracích tokenů najdete v těchto článku:

- [Nároky v přístupových tokenech](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Nároky na id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Nároky,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) které můžete očekávat v ID tokenech a přístupových tokenech vydaných Azure AD B2C
- [Referenční informace o deklarace tokenů SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
