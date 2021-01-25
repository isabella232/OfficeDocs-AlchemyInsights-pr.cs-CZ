---
title: Problémy s vývojem aplikací s rozhraním API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974382"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="c7ddf-102">Problémy s vývojem aplikací s rozhraním API</span><span class="sxs-lookup"><span data-stu-id="c7ddf-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="c7ddf-103">Pokud chcete začít používat aplikaci Azure Active Directory Graph API, podívejte se na [Příručka Začínáme s API Azure AD graphu](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) nebo si prohlédněte [interaktivní dokumentaci k rozhraní API Azure AD](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="c7ddf-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="c7ddf-104">**Konec podpory knihovny služby Azure Active Directory (ADAL) a rozhraní API Azure AD Graph (graf AAD)**</span><span class="sxs-lookup"><span data-stu-id="c7ddf-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="c7ddf-105">**Od června 2020** se už nepřidáme žádné nové funkce do grafu ADAL a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="c7ddf-106">Budeme dál poskytovat technické podpory a aktualizace zabezpečení, ale nebudete už poskytovat aktualizace funkcí.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="c7ddf-107">**Od června 2022** se vám ukončí podpora pro graf ADAL a Azure AD a nebudete už poskytovat technickou podporu ani aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="c7ddf-108">Aplikace používající ADAL v existujících verzích OS budou po této době dál fungovat, ale nezískají žádné technické podpory ani aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="c7ddf-109">Aplikace používající graf Azure AD už po této době nemusí přijímat odpovědi z koncového bodu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="c7ddf-110">**ADAL – migrace**</span><span class="sxs-lookup"><span data-stu-id="c7ddf-110">**ADAL Migration**</span></span>

<span data-ttu-id="c7ddf-111">Doporučujeme aktualizovat [knihovnu Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="c7ddf-112">Pokud používáte Microsoft Apps, je třeba vědět, že společnost Microsoft provádí migraci svých aplikací na MSAL pomocí konečného termínu poskytnutí podpory, což zajistí, že budou těžit ze služby MSAL a vylepšení funkcí.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="c7ddf-113">[Přečtěte si téma Nejčastější dotazy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="c7ddf-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="c7ddf-114">[Přečtěte si, jak migrovat aplikace na jednotlivých platformách](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="c7ddf-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="c7ddf-115">Pokud potřebujete pomoct s porozuměním, které z vašich aplikací používá ADAL, doporučujeme, abyste si provedli kontrolu všech zdrojových kódů a případně poskytovatelů ISV nebo aplikací.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="c7ddf-116">Podpora Microsoftu vám taky poskytne seznam všech aplikací ADAL, které nejsou od Microsoftu, ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="c7ddf-117">**Migrace grafu AAD**</span><span class="sxs-lookup"><span data-stu-id="c7ddf-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="c7ddf-118">U aplikací, které používají graf Azure AD, postupujte podle pokynů k migraci [aplikací Graph AD služby Azure do Microsoft graphu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="c7ddf-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="c7ddf-119">[Naše kontrolní seznam migrace představuje bod Začínáme](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="c7ddf-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="c7ddf-120">Portál registrace aplikací pro Azure zobrazuje, které aplikace používají graf AAD.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="c7ddf-121">Doporučujeme, abyste zkontrolovali všechny zdrojové kódy aplikací a pokud jsou k dispozici, a pokud je to možné, kontaktujte všechny poskytovatele ISV nebo aplikace.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="c7ddf-122">Podpora Microsoftu vám taky poskytne seznam všech použití grafu AAD ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="c7ddf-123">Aby aplikace Access mohla získat přístup k datům v Microsoft graphu, musí ji udělit správnému uživateli nebo správci.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="c7ddf-124">[Referenční informace o oprávnění Microsoft graphu](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) zobrazuje oprávnění spojená s jednotlivými hlavními skupinami rozhraní API Microsoft graphu.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="c7ddf-125">Poskytuje také pokyny, jak používat oprávnění.</span><span class="sxs-lookup"><span data-stu-id="c7ddf-125">It also provides guidance about how to use the permissions.</span></span>
