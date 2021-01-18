---
title: Výrazy SAML (tokeny)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884982"
---
# <a name="saml-assertions-tokens"></a>Výrazy SAML (tokeny)

1. Tokeny SAML (Security ASSERTS Language) jsou XML reprezentace deklarací. Ve výchozím nastavení jsou tokeny SAML používané službou WCF (Windows Communication Foundation) ve federovaných scénářích zabezpečení vydané tokeny. Další informace najdete v tématu [tokeny a deklarace SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Microsoft Identity Platform generuje několik typů tokenů zabezpečení při zpracování každého toku ověřování. [Deklarace tokenů SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) popisuje formát, zabezpečení a obsah tokenů SAML 2,0.
3. Podle pokynů v části [konfigurovatelného tokenu života v Microsoft Identity platformujte](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) , jak nakonfigurovat životnosti tokenů.
4. Postupujte podle kroků uvedených v [tomto článku](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) a zjistěte, jak nakonfigurovat šifrování tokenů služby Azure AD.
5. V Azure AD můžete nastavit možnosti podepisování certifikátů a algoritmus podepisování certifikátů. Další informace najdete v tématu [Rozšířené možnosti podepisování certifikátů v tokenu SAML pro aplikace Galerie v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
