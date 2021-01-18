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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="36a96-102">Výrazy SAML (tokeny)</span><span class="sxs-lookup"><span data-stu-id="36a96-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="36a96-103">Tokeny SAML (Security ASSERTS Language) jsou XML reprezentace deklarací.</span><span class="sxs-lookup"><span data-stu-id="36a96-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="36a96-104">Ve výchozím nastavení jsou tokeny SAML používané službou WCF (Windows Communication Foundation) ve federovaných scénářích zabezpečení vydané tokeny.</span><span class="sxs-lookup"><span data-stu-id="36a96-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="36a96-105">Další informace najdete v tématu [tokeny a deklarace SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="36a96-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="36a96-106">Microsoft Identity Platform generuje několik typů tokenů zabezpečení při zpracování každého toku ověřování.</span><span class="sxs-lookup"><span data-stu-id="36a96-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="36a96-107">[Deklarace tokenů SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) popisuje formát, zabezpečení a obsah tokenů SAML 2,0.</span><span class="sxs-lookup"><span data-stu-id="36a96-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="36a96-108">Podle pokynů v části [konfigurovatelného tokenu života v Microsoft Identity platformujte](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) , jak nakonfigurovat životnosti tokenů.</span><span class="sxs-lookup"><span data-stu-id="36a96-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="36a96-109">Postupujte podle kroků uvedených v [tomto článku](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) a zjistěte, jak nakonfigurovat šifrování tokenů služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="36a96-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="36a96-110">V Azure AD můžete nastavit možnosti podepisování certifikátů a algoritmus podepisování certifikátů.</span><span class="sxs-lookup"><span data-stu-id="36a96-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="36a96-111">Další informace najdete v tématu [Rozšířené možnosti podepisování certifikátů v tokenu SAML pro aplikace Galerie v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="36a96-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
