---
title: Práce s knihovnami ověřování
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
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035015"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="f5bc1-102">Práce s knihovnami ověřování</span><span class="sxs-lookup"><span data-stu-id="f5bc1-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="f5bc1-103">Pokud chcete vyřešit problém s knihovnou MSAL (Microsoft Authentication Library), proveďte následující doporučené kroky:</span><span class="sxs-lookup"><span data-stu-id="f5bc1-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="f5bc1-104">**Práce s rozhraním MSAL**: Knihovny ověřování [na platformě identit Microsoftu](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – tento článek ukazuje podporu knihovny microsoftového ověřování pro několik typů aplikací.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="f5bc1-105">Obsahuje odkazy na zdrojový kód knihovny. kde získat balíček pro projekt aplikace; a jestli knihovna podporuje přihlášení uživatele (ověřování), přístup k chráněným webovým rozhraním API (autorizace) nebo obojí.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="f5bc1-106">**Poradce při potížích** s ověřováním: Funkce MSAL podporuje několik toků ověřování pro použití v různých scénářích aplikací.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="f5bc1-107">V závislosti na tom, jak je vaše klientská aplikace vytvořená, může msal použít jeden nebo více toků ověřování podporovaných platformou identit Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="f5bc1-108">Tyto toky mohou vytvářet několik typů tokenů a autorizačních kódů a vyžadovat různé tokeny, aby fungovaly.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="f5bc1-109">**Přístupové tokeny:** [Přístupové tokeny platformy microsoftu](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – zjistěte, jak může rozhraní API ověřovat a používat deklarace identity uvnitř přístupového tokenu.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="f5bc1-110">Veškerá dokumentace v tomto článku, s výjimkou případů uvedených, platí jenom pro tokeny vydané pro rozhraní API, která jste zaregistrovali.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="f5bc1-111">Nevztahuje se na tokeny vydané pro rozhraní API vlastněné společností Microsoft a tyto tokeny se nedávají použít k ověření, jak bude platforma identit Microsoft vydávat tokeny pro rozhraní API, které vytvoříte.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="f5bc1-112">**Ukončení podpory knihovny ověřování služby Azure Active Directory (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="f5bc1-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="f5bc1-113">**Od 30. června 2020** už nebudeme přidávat žádné nové funkce do ADAL a Azure AD Graphu.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="f5bc1-114">Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="f5bc1-115">**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a už nebudeme poskytovat technickou podporu ani aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="f5bc1-116">Aplikace, které používají ADAL ve stávajících verzích operačního systému, budou i po této době fungovat, ale nebudou dostávat technickou podporu ani *aktualizace zabezpečení*.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="f5bc1-117">Aplikace používající Azure AD Graph po této době už nemusí přijímat odpovědi z koncového bodu Azure AD Graphu.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="f5bc1-118">**Migrace ADAL**</span><span class="sxs-lookup"><span data-stu-id="f5bc1-118">**ADAL Migration**</span></span>

- <span data-ttu-id="f5bc1-119">Doporučujeme aktualizovat na msal, který má nejnovější funkce a aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="f5bc1-120">Pokud používáte aplikace Microsoft, věrte, že Microsoft do konečného termínu ukončení podpory migruje své aplikace na MSAL, takže budou mít prospěch z průběžného zabezpečení a vylepšení funkcí msal.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="f5bc1-121">[Přečtěte si časté otázky k ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="f5bc1-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="f5bc1-122">[Přečtěte si, jak migrovat aplikace na platformě.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="f5bc1-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="f5bc1-123">Pokud po přečtení příručky pro platformu vaší aplikace máte další otázky, můžete příspěvek na [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) se značkou [azure-ad-adal-deprecation] nebo otevřít problém v úložišti GitHubu knihovny.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="f5bc1-124">Odkazy [na repo](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) knihovny najdete v části Jazyky a rámce v článku přehledu **MSAL.**</span><span class="sxs-lookup"><span data-stu-id="f5bc1-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="f5bc1-125">**Pokud potřebujete pomoct s pochopením, které aplikace používají ADAL,** doporučujeme zkontrolovat zdrojový kód všech aplikací.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="f5bc1-126">Pokud je to možné, můžete kontaktovat nezávislé dodavatele softwaru (ISV) nebo poskytovatele aplikací.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="f5bc1-127">Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="f5bc1-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







