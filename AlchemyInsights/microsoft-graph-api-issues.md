---
title: Problémy s rozhraním Microsoft Graph API
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713470"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="0b442-102">Problémy s rozhraním Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="0b442-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="0b442-103">Toto téma se může také vztahovat na vývojáře, kteří stále používají rozhraní Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="0b442-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="0b442-104">Důrazně ale **doporučujeme** používat Microsoft Graph pro všechny scénáře správy adresářů, identit a přístupu.</span><span class="sxs-lookup"><span data-stu-id="0b442-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="0b442-105">**Problémy s ověřováním nebo autorizacem**</span><span class="sxs-lookup"><span data-stu-id="0b442-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="0b442-106">Pokud aplikace nemůže získat **tokeny,** které volají na Microsoft Graph, vyberte Problém se získáním kategorie Microsoft **Graphu pro přístupový token (ověřování),** abyste získali konkrétnější nápovědu a podporu pro toto téma.</span><span class="sxs-lookup"><span data-stu-id="0b442-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="0b442-107">Pokud aplikace dostává při volání Microsoft Graphu chyby autorizace **401 nebo 403,** vyberte kategorii Získání chyby odepření přístupu **(autorizace)** rozhraní Microsoft Graph API, abyste získali konkrétnější nápovědu a podporu k tomuto tématu.</span><span class="sxs-lookup"><span data-stu-id="0b442-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="0b442-108">**Chci používat Microsoft Graph, ale nevím, kde začít**</span><span class="sxs-lookup"><span data-stu-id="0b442-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="0b442-109">Základní informace o Microsoft Graphu</span><span class="sxs-lookup"><span data-stu-id="0b442-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="0b442-110">Přehled správy identit a přístupu v aplikaci Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0b442-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="0b442-111">Začínáme s vytvářením aplikací Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0b442-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="0b442-112">**Microsoft Graph Explorer** – Testování rozhraní Microsoft Graph API ve vašem tenantovi nebo ukázkovém tenantovi</span><span class="sxs-lookup"><span data-stu-id="0b442-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="0b442-113">**Chci používat Microsoft Graph, ale podporuje rozhraní API adresáře v1.0, která potřebuji?**</span><span class="sxs-lookup"><span data-stu-id="0b442-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="0b442-114">Microsoft Graph je doporučené rozhraní API pro správu adresáře, identity a přístupu.</span><span class="sxs-lookup"><span data-stu-id="0b442-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="0b442-115">Mezi tím, co je možné v Azure AD Graphu a Microsoft Graphu, je ale pořád pár mezer.</span><span class="sxs-lookup"><span data-stu-id="0b442-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="0b442-116">Projděte si následující články, ve kterých jsou uvedené nejnovější rozdíly, které vám pomohou při výběru:</span><span class="sxs-lookup"><span data-stu-id="0b442-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="0b442-117">Rozdíly typů zdrojů mezi Azure AD Graph a Microsoft Graphem</span><span class="sxs-lookup"><span data-stu-id="0b442-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="0b442-118">Rozdíly ve vlastnostech mezi Azure AD Graph a Microsoft Graphem</span><span class="sxs-lookup"><span data-stu-id="0b442-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="0b442-119">Rozdíly mezi metodami mezi Azure AD a Microsoft Graphem</span><span class="sxs-lookup"><span data-stu-id="0b442-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="0b442-120">**Rozhraní API, které volám, nefunguje – kde můžu dělat další testování?**</span><span class="sxs-lookup"><span data-stu-id="0b442-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="0b442-121">**Microsoft Graph Explorer** – Otestujte rozhraní Microsoft Graph API ve vašem tenantovi nebo ukázkovém tenantovi a také se podívejte na ukázkové dotazy **v** Microsoft Graph Exploreru.</span><span class="sxs-lookup"><span data-stu-id="0b442-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="0b442-122">**Moje aplikace je příliš pomalá a zároveň se zhroucela. Jaká vylepšení můžu udělat?**</span><span class="sxs-lookup"><span data-stu-id="0b442-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="0b442-123">V závislosti na vašem scénáři se k dispozici různé možnosti, jak zajistit výkon aplikace, a v některých případech je méně náchylná k omezení služby (když provádíte příliš mnoho hovorů).</span><span class="sxs-lookup"><span data-stu-id="0b442-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="0b442-124">Doporučené postupy pro Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0b442-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="0b442-125">Žádosti o dávku</span><span class="sxs-lookup"><span data-stu-id="0b442-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="0b442-126">Sledování změn prostřednictvím rozdílového dotazu</span><span class="sxs-lookup"><span data-stu-id="0b442-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="0b442-127">Oznámení o změnách prostřednictvím webhooků</span><span class="sxs-lookup"><span data-stu-id="0b442-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="0b442-128">Pokyny pro omezení</span><span class="sxs-lookup"><span data-stu-id="0b442-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="0b442-129">**Kde najdu další informace o chybách a známých problémech?**</span><span class="sxs-lookup"><span data-stu-id="0b442-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="0b442-130">Informace o odpovědi na chyby v Microsoft Graphu</span><span class="sxs-lookup"><span data-stu-id="0b442-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="0b442-131">Známé problémy s Microsoft Graphem</span><span class="sxs-lookup"><span data-stu-id="0b442-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="0b442-132">**Kde můžu zkontrolovat stav dostupnosti a připojení služeb?**</span><span class="sxs-lookup"><span data-stu-id="0b442-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="0b442-133">Dostupnost služeb a připojení základních služeb, ke kterým se můžete dostat přes Microsoft Graph, může mít vliv na celkovou dostupnost a výkon Microsoft Graphu.</span><span class="sxs-lookup"><span data-stu-id="0b442-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="0b442-134">Pokud chcete zjistit stav služby Azure Active Directory, zkontrolujte stav služeb **Security + Identity,** které jsou uvedené na [stránce stavu Azure.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="0b442-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="0b442-135">U služeb Office, které do Microsoft Graphu přispívají, se podívejte na stav služeb uvedených na řídicím panelu [stavu služeb Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="0b442-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="0b442-136">Chyby autorizace Aplikace Microsoft Graph mohou být výsledkem několika různých problémů, z nichž většina vygeneruje chybu 401 nebo 403.</span><span class="sxs-lookup"><span data-stu-id="0b442-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="0b442-137">Například následující příklad může vést k chybám autorizace:</span><span class="sxs-lookup"><span data-stu-id="0b442-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="0b442-138">Nesprávné [toky akvizice přístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="0b442-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="0b442-139">Špatně nakonfigurované [rozsahy oprávnění](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="0b442-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="0b442-140">Chybějící [souhlas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="0b442-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="0b442-141">\**_Konec podpory pro knihovnu Azure Active Directory Authentication Library (ADAL) a rozhraní API Azure AD Graph (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="0b442-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="0b442-142">_*Od 30. června 2020*\* nebudeme do ADAL a Azure AD Graph přidávat žádné nové funkce.</span><span class="sxs-lookup"><span data-stu-id="0b442-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="0b442-143">Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.</span><span class="sxs-lookup"><span data-stu-id="0b442-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="0b442-144">**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a nebudeme už poskytovat technickou podporu ani aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="0b442-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="0b442-145">Aplikace používající ADAL ve stávajících verzích operačního systému budou i po této době dál fungovat, ale nebudou dostávat žádné aktualizace technické podpory ani *zabezpečení.*</span><span class="sxs-lookup"><span data-stu-id="0b442-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="0b442-146">Aplikace používající Azure AD Graph po této době už nemusí dostávat odpovědi z koncového bodu Azure AD Graphu.</span><span class="sxs-lookup"><span data-stu-id="0b442-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="0b442-147">**Migrace ADAL**</span><span class="sxs-lookup"><span data-stu-id="0b442-147">**ADAL Migration**</span></span>

<span data-ttu-id="0b442-148">Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="0b442-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="0b442-149">Pokud používáte aplikace Microsoftu, věděli jste, že Microsoft do konečného termínu ukončení podpory migruje aplikace na msal, a zajišťuje tak, že pro msAL budou využívat průběžná vylepšení zabezpečení a funkcí.</span><span class="sxs-lookup"><span data-stu-id="0b442-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="0b442-150">Přečtěte si časté otázky k ADAL</span><span class="sxs-lookup"><span data-stu-id="0b442-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="0b442-151">Informace o tom, jak migrovat aplikace na základě platformy</span><span class="sxs-lookup"><span data-stu-id="0b442-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="0b442-152">Pokud potřebujete pomoct s pochopením, která z vašich aplikací používá ADAL, doporučujeme zkontrolovat si zdrojový kód všech aplikací, a pokud je to možné, kontaktovat některé isVs nebo poskytovatele aplikací.</span><span class="sxs-lookup"><span data-stu-id="0b442-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="0b442-153">Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="0b442-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="0b442-154">**Migrace AAD Graphu**</span><span class="sxs-lookup"><span data-stu-id="0b442-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="0b442-155">U aplikací, které používají Azure AD Graph, postupujte podle pokynů k migraci aplikací [Azure AD Graph do Microsoft Graphu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="0b442-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="0b442-156">[Základní informace najdete v našem kontrolním seznamu migrace](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="0b442-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="0b442-157">Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure.</span><span class="sxs-lookup"><span data-stu-id="0b442-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="0b442-158">Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací.</span><span class="sxs-lookup"><span data-stu-id="0b442-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="0b442-159">Podpora Microsoftu vám také může poskytnout seznam všech využití AAD Graphu ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="0b442-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="0b442-160">Aby vaše aplikace získá přístup k datům v Microsoft Graphu, musí ji uživatel nebo správce udělit správná oprávnění prostřednictvím procesu udělení souhlasu.</span><span class="sxs-lookup"><span data-stu-id="0b442-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="0b442-161">Odkaz [na oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference) obsahuje oprávnění přidružená k jednotlivým hlavním sadě rozhraní Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="0b442-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="0b442-162">Obsahuje taky pokyny, jak tato oprávnění používat.</span><span class="sxs-lookup"><span data-stu-id="0b442-162">It also provides guidance about how to use the permissions.</span></span>
