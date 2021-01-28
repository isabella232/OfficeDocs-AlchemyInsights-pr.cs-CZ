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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="33074-102">Problémy s atributy a deklarace tokenů</span><span class="sxs-lookup"><span data-stu-id="33074-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="33074-103">**Aktualizace, konfigurace nebo odebrání deklarace tokenů**</span><span class="sxs-lookup"><span data-stu-id="33074-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="33074-104">Pomocí Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD) můžete přizpůsobit typ deklarace identity pro claim role v tokenu pro odpověď, který dostanete po autorizaci aplikace.</span><span class="sxs-lookup"><span data-stu-id="33074-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="33074-105">Vývojáři aplikací mohou ve svých aplikacích Azure AD používat volitelné nároky k určení toho, jaké nároky chtějí mít v tokenech posílaných do své aplikace.</span><span class="sxs-lookup"><span data-stu-id="33074-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="33074-106">Další informace najdete v článku [Poskytnutí nepovinných](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)nároků ve vaší aplikaci.</span><span class="sxs-lookup"><span data-stu-id="33074-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="33074-107">[Nakonfigurujte deklarace skupin pro aplikace pomocí Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="33074-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="33074-108">Pokud používáte bezproblémové jednotné přihlašování ve vaší aplikaci, podívejte se na přizpůsobení nároků vydaných [v tokenu SAML pro podnikové aplikace.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="33074-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="33074-109">**Mapování atributů deklarací**</span><span class="sxs-lookup"><span data-stu-id="33074-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="33074-110">Pokud chcete nakonfigurovat zásady mapování deklarací identity pomocí PowerShellu, podívejte se na stránku Přizpůsobení deklarací identity sílané do tokenů konkrétní aplikace v [tenantovi (Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="33074-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="33074-111">Atributy rozšíření schématu adresáře umožňují ukládat do Azure Active Directory další data v objektech uživatelů a jiných adresářových objektech, jako jsou skupiny, podrobnosti o tenantovi a objekty zabezpečení služby.</span><span class="sxs-lookup"><span data-stu-id="33074-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="33074-112">K uplatnění nároku na nároky na aplikace lze použít pouze atributy rozšíření u uživatelských objektů.</span><span class="sxs-lookup"><span data-stu-id="33074-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="33074-113">[Použití atributů rozšíření schématu adresáře v claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) popisuje, jak používat atributy rozšíření schématu adresáře pro odesílání uživatelských dat aplikacím v deklaracích tokenů.</span><span class="sxs-lookup"><span data-stu-id="33074-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="33074-114">Další informace o deklaracích tokenů najdete v těchto článku:</span><span class="sxs-lookup"><span data-stu-id="33074-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="33074-115">Nároky v přístupových tokenech</span><span class="sxs-lookup"><span data-stu-id="33074-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="33074-116">Nároky na id_token</span><span class="sxs-lookup"><span data-stu-id="33074-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="33074-117">[Nároky,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) které můžete očekávat v ID tokenech a přístupových tokenech vydaných Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="33074-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="33074-118">Referenční informace o deklarace tokenů SAML</span><span class="sxs-lookup"><span data-stu-id="33074-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
