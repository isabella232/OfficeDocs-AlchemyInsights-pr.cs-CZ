---
title: Problémy s deklaracemi tokenů a atributy
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
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012877"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problémy s deklaracemi tokenů a atributy

**Aktualizace, konfigurace nebo odebrání deklarací tokenu**

1. Pomocí Azure Active Directory (Azure AD) můžete [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) přizpůsobit typ deklarace identity pro deklaraci role v tokenu odpovědi, který obdržíte po autorizaci aplikace.
2. Vývojáři aplikací mohou v aplikacích Azure AD používat volitelné deklarace identity k určení, které deklarace identity chtějí v tokenech odeslaných do jejich aplikace. Další informace najdete v tématu [Poskytnutí volitelných deklarací identity do aplikace](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigurace deklarací skupiny pro aplikace pomocí Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Pokud v aplikaci používáte bezproblémové jednotné přihlašování, podívejte se na informace v tématu Přizpůsobení deklarací vydaných [v tokenu SAML pro podnikové aplikace](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Mapování atributů deklarací identity**

1. Informace o konfiguraci zásad mapování deklarací identity pomocí PowerShellu najdete v tématu Přizpůsobení deklarací identity vydávané v tokenech pro konkrétní [aplikaci v tenantovi (Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atributy rozšíření schématu adresáře umožňují ukládat další data v Azure Active Directory objektů uživatelů a dalších objektů adresáře, jako jsou skupiny, podrobnosti tenanta, objekty služby. K vysílání deklarací do aplikací se používejte jenom atributy rozšíření u uživatelských objektů. [Použití atributů rozšíření schématu adresáře](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) v deklaracích identity popisuje, jak používat atributy rozšíření schématu adresáře pro odesílání uživatelských dat do aplikací v deklaracích tokenů.

Další informace o deklaracích tokenů najdete v těchto tématu:

- [Deklarace identity v přístupových tokenech](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Nároky v id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Deklarace identity,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) které můžete očekávat v tokenech ID a přístupových tokenech vydaných Službou Azure AD B2C
- [Odkaz na deklarace tokenů SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
