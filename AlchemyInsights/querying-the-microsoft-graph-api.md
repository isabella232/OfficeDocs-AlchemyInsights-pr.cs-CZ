---
title: Dotazování rozhraní Microsoft Graph API
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974216"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="76a76-102">Dotazování rozhraní Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="76a76-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="76a76-103">Toto téma se taky bude vztahovat na vývojáře, kteří ještě používají API Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="76a76-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="76a76-104">Ve scénářích pro správu adresářů, identit a Access se ale **důrazně** doporučuje používat Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="76a76-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="76a76-105">**Problémy s ověřováním nebo autorizací**</span><span class="sxs-lookup"><span data-stu-id="76a76-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="76a76-106">Pokud se vaší aplikací **nepodaří získat tokeny** pro volání do aplikace Microsoft Graph, vyberte **problém se získáním přístupového tokenu (Authentication)** kategorie Microsoft graphu a získejte konkrétnější nápovědu a podporu k tomuto tématu.</span><span class="sxs-lookup"><span data-stu-id="76a76-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="76a76-107">Pokud se při volání Microsoft graphu aplikace dostanou **chyby autorizace 401 nebo 403** , vyberte v části **získání chyby odepření přístupu (autorizace)** kategorii Microsoft Graph API pro získání přesnější nápovědy a podpory k tomuto tématu.</span><span class="sxs-lookup"><span data-stu-id="76a76-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="76a76-108">**Chci používat Microsoft Graph, ale nevíte, kde začít**</span><span class="sxs-lookup"><span data-stu-id="76a76-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="76a76-109">Další informace o aplikaci Microsoft Graph naleznete v tématech:</span><span class="sxs-lookup"><span data-stu-id="76a76-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="76a76-110">Přehled aplikace Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76a76-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="76a76-111">Základní informace o správě identit a přístupu v Microsoft graphu</span><span class="sxs-lookup"><span data-stu-id="76a76-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="76a76-112">Začínáme s vytvářením aplikací Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76a76-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="76a76-113">**Průzkumník Microsoft graphu** – testování rozhraní Microsoft Graph API v tenantovi nebo ukázkovém tenantovi</span><span class="sxs-lookup"><span data-stu-id="76a76-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="76a76-114">**Chci používat Microsoft Graph, ale podporuje rozhraní API v adresáři verze 1.0?**</span><span class="sxs-lookup"><span data-stu-id="76a76-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="76a76-115">Doporučeným rozhraním API pro správu adresářů, identit a přístupu je Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="76a76-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="76a76-116">V grafu Azure AD a v Microsoft graphu je ale pořád pár mezer.</span><span class="sxs-lookup"><span data-stu-id="76a76-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="76a76-117">Přečtěte si následující články, které by měly zvýraznit nejaktuálnější rozdíly, které vám umožní váš výběr:</span><span class="sxs-lookup"><span data-stu-id="76a76-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="76a76-118">Rozdíly mezi typy zdrojů v Azure AD graphu a Microsoft graphu</span><span class="sxs-lookup"><span data-stu-id="76a76-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="76a76-119">Rozdíly mezi vlastnostmi v Azure AD graphu a Microsoft graphu</span><span class="sxs-lookup"><span data-stu-id="76a76-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="76a76-120">Rozdíly mezi metodami v Azure AD a Microsoft graphu</span><span class="sxs-lookup"><span data-stu-id="76a76-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="76a76-121">**Při dotazování objektu *uživatele* chybí mnoho jeho vlastností**</span><span class="sxs-lookup"><span data-stu-id="76a76-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="76a76-122">`GET https://graph.microsoft.com/v1.0/users` Vrátí jenom 11 vlastností, protože Microsoft Graph automaticky vybere výchozí sadu *uživatelských* vlastností, které se mají vrátit.</span><span class="sxs-lookup"><span data-stu-id="76a76-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="76a76-123">Pokud potřebujete další vlastnosti *uživatelů* , vyberte pomocí $Select vlastnosti, které aplikace potřebuje.</span><span class="sxs-lookup"><span data-stu-id="76a76-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="76a76-124">Vyzkoušejte nejprve v **aplikaci Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="76a76-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="76a76-125">**Některé hodnoty vlastností uživatele jsou *prázdné* , i když vím, že jsou nastavené.**</span><span class="sxs-lookup"><span data-stu-id="76a76-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="76a76-126">Nejpravděpodobnější vysvětlení je, že aplikaci bylo udělené oprávnění *User. ReadBasic. All* .</span><span class="sxs-lookup"><span data-stu-id="76a76-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="76a76-127">To umožňuje aplikaci číst omezenou sadu uživatelských vlastností a vracet tak všechny ostatní vlastnosti jako hodnoty null, a to i v případě, že byly dříve nastavené.</span><span class="sxs-lookup"><span data-stu-id="76a76-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="76a76-128">Zkuste udělit oprávnění *uživatele aplikace. Read. All* .</span><span class="sxs-lookup"><span data-stu-id="76a76-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="76a76-129">Další informace najdete v článku [uživatelská oprávnění aplikace Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="76a76-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="76a76-130">**Mám potíže s použitím parametrů dotazu OData k filtrování dat v mých žádostech**</span><span class="sxs-lookup"><span data-stu-id="76a76-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="76a76-131">Zatímco Microsoft Graph podporuje široký rozsah parametrů dotazu OData, mnohé z těchto parametrů nejsou plně podporované adresářovými službami (prostředky, které dědí z *directoryObject*) v Microsoft graphu.</span><span class="sxs-lookup"><span data-stu-id="76a76-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="76a76-132">Stejná omezení, která byla uložena v Azure AD grafu ve většině částí aplikace Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="76a76-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="76a76-133">**Nepodporované**: $count, $search a *$Filter na hodnoty null* nebo *NOT NULL*</span><span class="sxs-lookup"><span data-stu-id="76a76-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="76a76-134">**Nepodporované**: $Filter na určitých vlastnostech (viz témata o zdrojích, na kterých se dají filtrovat vlastnosti)</span><span class="sxs-lookup"><span data-stu-id="76a76-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="76a76-135">**Nepodporované**: stránkování, filtrování a řazení najednou</span><span class="sxs-lookup"><span data-stu-id="76a76-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="76a76-136">**Nepodporuje se**: filtrování podle vztahu.</span><span class="sxs-lookup"><span data-stu-id="76a76-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="76a76-137">Můžete například najít všechny členy technické skupiny, kteří jsou ve Velké Británii.</span><span class="sxs-lookup"><span data-stu-id="76a76-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="76a76-138">**Částečná podpora**: $OrderBy pro *uživatele* (jenom DisplayName a userPrincipalName) a *skupiny*</span><span class="sxs-lookup"><span data-stu-id="76a76-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="76a76-139">**Částečná podpora**: $Filter (podporuje jenom *EQ*, *StartsWith* *nebo* a *omezená* *jakákoli*), $expand (rozbalení relací jednoho objektu vrátí všechny relace, ale rozbalování relací objektů je omezené)</span><span class="sxs-lookup"><span data-stu-id="76a76-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="76a76-140">Další informace najdete v tématu [přizpůsobení odpovědí pomocí parametrů dotazu](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="76a76-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="76a76-141">**Rozhraní API, které já zavolám nefunguje – kde můžu dělat další testování?**</span><span class="sxs-lookup"><span data-stu-id="76a76-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="76a76-142">**Průzkumník Microsoft graphu** – otestujte rozhraní API Microsoft graphu ve vašem tenantovi nebo ukázkovém tenantovi a podívejte se také na **Ukázkové dotazy** v aplikaci Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="76a76-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="76a76-143">**Když se dotazovat na data, zdá se, že mám nekompletní sadu dat**</span><span class="sxs-lookup"><span data-stu-id="76a76-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="76a76-144">Pokud vytváříte dotazování na kolekci (například *Uživatelé*), používá Microsoft Graph limit stránek na straně serveru, takže výsledky jsou vždycky vráceny s výchozí velikostí stránky.</span><span class="sxs-lookup"><span data-stu-id="76a76-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="76a76-145">Aplikace by měla vždy očekávat, že budou stránky ze sběru vrácené službou.</span><span class="sxs-lookup"><span data-stu-id="76a76-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="76a76-146">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="76a76-146">For more information, see:</span></span>

- [<span data-ttu-id="76a76-147">Doporučené postupy pro Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76a76-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="76a76-148">Stránkování dat aplikace Microsoft Graph ve vaší aplikaci</span><span class="sxs-lookup"><span data-stu-id="76a76-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="76a76-149">**Moje aplikace je moc pomalá a zároveň zobrazuje omezení. Jaká vylepšení můžu dělat?**</span><span class="sxs-lookup"><span data-stu-id="76a76-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="76a76-150">V závislosti na tom, jaký máte váš scénář, máte k dispozici nejrůznější různé možnosti, díky kterým bude aplikace pracovat, a v některých případech méně náchylné k omezení služby (při provádění příliš mnoha hovorů).</span><span class="sxs-lookup"><span data-stu-id="76a76-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="76a76-151">Více k tomu najdete tady:</span><span class="sxs-lookup"><span data-stu-id="76a76-151">To learn more, see:</span></span>

- [<span data-ttu-id="76a76-152">Doporučené postupy pro Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76a76-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="76a76-153">Žádosti o dávkové zpracování</span><span class="sxs-lookup"><span data-stu-id="76a76-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="76a76-154">Sledování změn v rozdílovém dotazu</span><span class="sxs-lookup"><span data-stu-id="76a76-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="76a76-155">Upozornění na změny prostřednictvím webhooků</span><span class="sxs-lookup"><span data-stu-id="76a76-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="76a76-156">Pokyny pro omezení</span><span class="sxs-lookup"><span data-stu-id="76a76-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="76a76-157">**Kde najdu Další informace o chybách a známých problémech?**</span><span class="sxs-lookup"><span data-stu-id="76a76-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="76a76-158">Informace o chybové odezvě Microsoft graphu</span><span class="sxs-lookup"><span data-stu-id="76a76-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="76a76-159">Známé problémy s Microsoft graphem</span><span class="sxs-lookup"><span data-stu-id="76a76-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="76a76-160">**Kde můžu zkontrolovat stav dostupnosti služeb a připojení?**</span><span class="sxs-lookup"><span data-stu-id="76a76-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="76a76-161">Dostupnost a připojení základních služeb, ke kterým lze získat přístup pomocí aplikace Microsoft Graph, může ovlivnit celkovou dostupnost a výkon aplikace Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="76a76-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="76a76-162">Pro stav služby Azure Active Directory zkontrolujte stav služby **Security + Identity** uvedené na [stránce Stav Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="76a76-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="76a76-163">V případě služeb Office, které přispívají do aplikace Microsoft Graph, zkontrolujte stav služeb uvedených na [řídicím panelu stavu služby Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="76a76-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
