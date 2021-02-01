---
title: Problémy s knihovnami ověřování
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063588"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="70fad-102">Problémy s knihovnami ověřování</span><span class="sxs-lookup"><span data-stu-id="70fad-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="70fad-103">[Knihovny ověřování platformy](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identit Microsoft uvádí knihovny klientů a middleware podporovaných a kompatibilními společností Microsoft.</span><span class="sxs-lookup"><span data-stu-id="70fad-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="70fad-104">Knihovna MSAL (Microsoft Authentication Library) podporuje několik ověřovacích [toků](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) pro použití v různých scénářích aplikací.</span><span class="sxs-lookup"><span data-stu-id="70fad-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="70fad-105">K ověření a získání tokenů můžete v kódu inicializovat novou veřejnou nebo důvěrnou klientskou aplikaci.</span><span class="sxs-lookup"><span data-stu-id="70fad-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="70fad-106">Při inicializaci klientské aplikace v Knihovně ověřování Microsoft (MSAL) můžete nastavit několik možností konfigurace.</span><span class="sxs-lookup"><span data-stu-id="70fad-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="70fad-107">Další informace najdete v části [Možnosti konfigurace aplikace.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="70fad-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="70fad-108">**Ukončení podpory knihovny ADAL (Azure Active Directory Authentication Library) a rozhraní Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="70fad-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="70fad-109">**Od 30. června 2020** už do ADAL a Azure AD Graphu nebudeme přidávat nové funkce.</span><span class="sxs-lookup"><span data-stu-id="70fad-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="70fad-110">Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.</span><span class="sxs-lookup"><span data-stu-id="70fad-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="70fad-111">**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a nebudeme už poskytovat technickou podporu ani aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="70fad-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="70fad-112">Aplikace používající ADAL ve stávajících verzích operačního systému budou i po této době dál fungovat, ale nebudou dostávat žádné aktualizace technické podpory ani *zabezpečení.*</span><span class="sxs-lookup"><span data-stu-id="70fad-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="70fad-113">Aplikace používající Azure AD Graph po této době už nemusí dostávat odpovědi z koncového bodu Azure AD Graphu.</span><span class="sxs-lookup"><span data-stu-id="70fad-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="70fad-114">**Migrace ADAL**</span><span class="sxs-lookup"><span data-stu-id="70fad-114">**ADAL Migration**</span></span>

<span data-ttu-id="70fad-115">Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="70fad-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="70fad-116">Pokud používáte aplikace Microsoftu, věděli jste, že Microsoft ve výchozím nastavení migruje aplikace do systému MSAL do konečného termínu ukončení podpory, takže pro něj bude výhodná průběžná vylepšení zabezpečení a funkcí pro MSAL.</span><span class="sxs-lookup"><span data-stu-id="70fad-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="70fad-117">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="70fad-117">For more information, see:</span></span>

1. [<span data-ttu-id="70fad-118">Přečtěte si časté otázky k ADAL</span><span class="sxs-lookup"><span data-stu-id="70fad-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="70fad-119">Informace o tom, jak migrovat aplikace na základě platformy</span><span class="sxs-lookup"><span data-stu-id="70fad-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="70fad-120">Pokud potřebujete pomoct s pochopením, která z vašich aplikací používá ADAL, doporučujeme zkontrolovat si zdrojový kód všech aplikací, a pokud je to možné, kontaktovat některé isVs nebo poskytovatele aplikací.</span><span class="sxs-lookup"><span data-stu-id="70fad-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="70fad-121">Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="70fad-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="70fad-122">**Migrace AAD Graphu**</span><span class="sxs-lookup"><span data-stu-id="70fad-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="70fad-123">U aplikací, které používají Azure AD Graph, postupujte podle pokynů k migraci aplikací [Azure AD Graph do Microsoft Graphu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="70fad-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="70fad-124">Kontrolní seznam migrace nabízí základní informace.</span><span class="sxs-lookup"><span data-stu-id="70fad-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="70fad-125">Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure.</span><span class="sxs-lookup"><span data-stu-id="70fad-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="70fad-126">Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací.</span><span class="sxs-lookup"><span data-stu-id="70fad-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="70fad-127">Podpora Microsoftu vám také může poskytnout seznam všech využití AAD Graphu ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="70fad-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="70fad-128">Aby vaše aplikace získá přístup k datům v Microsoft Graphu, musí ji uživatel nebo správce udělit správná oprávnění prostřednictvím procesu udělení souhlasu.</span><span class="sxs-lookup"><span data-stu-id="70fad-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="70fad-129">Odkaz [na oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference) obsahuje oprávnění přidružená k jednotlivým hlavním sadě rozhraní Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="70fad-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="70fad-130">Obsahuje taky pokyny, jak tato oprávnění používat.</span><span class="sxs-lookup"><span data-stu-id="70fad-130">It also provides guidance about how to use the permissions.</span></span>
