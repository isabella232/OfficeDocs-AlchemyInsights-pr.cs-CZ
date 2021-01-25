---
title: Problémy s vývojem aplikací
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974229"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="a6292-102">Problémy s vývojem aplikací</span><span class="sxs-lookup"><span data-stu-id="a6292-102">Issues developing applications</span></span>

<span data-ttu-id="a6292-103">Pokud chcete vyřešit nejběžnější problémy při vytváření aplikací služby Azure Active Directory (AD), podívejte se na následující články:</span><span class="sxs-lookup"><span data-stu-id="a6292-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="a6292-104">Mám potíže s přihlášením k aplikacím pomocí prohlížeče Chrome</span><span class="sxs-lookup"><span data-stu-id="a6292-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="a6292-105">Nevím, jak změnit výchozí hodnoty životnosti tokenů pro aplikaci</span><span class="sxs-lookup"><span data-stu-id="a6292-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="a6292-106">Myslím, jak funguje souhlas s aplikací</span><span class="sxs-lookup"><span data-stu-id="a6292-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="a6292-107">Nevím, jak udělit oprávnění k aplikaci</span><span class="sxs-lookup"><span data-stu-id="a6292-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="a6292-108">Nerozumím rozdílu mezi delegovanými a oprávněními aplikací</span><span class="sxs-lookup"><span data-stu-id="a6292-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="a6292-109">\***Konec podpory knihovny služby Azure Active Directory (ADAL) a rozhraní API služby Azure AD Graph (graf AAD)** _</span><span class="sxs-lookup"><span data-stu-id="a6292-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="a6292-110">Po zahájení června 2020 nepřidáme do knihovny Azure Active Directory Authentication Library (ADAL) a rozhraní API Azure AD graphu žádné nové funkce.</span><span class="sxs-lookup"><span data-stu-id="a6292-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="a6292-111">Budeme dál poskytovat technické podpory a aktualizace zabezpečení, ale nebudete už poskytovat aktualizace funkcí.</span><span class="sxs-lookup"><span data-stu-id="a6292-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="a6292-112">Od června 2022, my vám ukončí podporu pro graf ADAL a AAD a nebude už poskytovat technickou podporu ani aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="a6292-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="a6292-113">V důsledku této podmínky jsou tyto důsledky:</span><span class="sxs-lookup"><span data-stu-id="a6292-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="a6292-114">Aplikace používající ADAL v existujících verzích OS budou po této době dál fungovat, ale nezískají žádné technické podpory ani aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="a6292-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="a6292-115">Aplikace používající graf AAD po této době už nemusí přijímat odpovědi z koncového bodu grafu AAD.</span><span class="sxs-lookup"><span data-stu-id="a6292-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="a6292-116">_ *Migrace*\*</span><span class="sxs-lookup"><span data-stu-id="a6292-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="a6292-117">Pokud používáte aplikace Microsoftu, doporučujeme aktualizovat knihovnu Microsoft Authentication Library (MSAL), která obsahuje nejnovější funkce a aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="a6292-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="a6292-118">Toto doporučení je v souvislosti se společností Microsoft zahajující proces migrace jeho aplikací na MSAL pomocí konečného termínu ukončení podpory.</span><span class="sxs-lookup"><span data-stu-id="a6292-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="a6292-119">Migrace společností Microsoft svých aplikací na MSAL zajišťuje, aby aplikace využily výhody vylepšeného zabezpečení a funkcí MSAL.</span><span class="sxs-lookup"><span data-stu-id="a6292-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="a6292-120">Přečtěte si část časté otázky</span><span class="sxs-lookup"><span data-stu-id="a6292-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="a6292-121">Informace o migraci aplikací na základě jednotlivých platforem</span><span class="sxs-lookup"><span data-stu-id="a6292-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="a6292-122">Pokud potřebujete pomoct s pochopením, které aplikace používají ADAL, doporučujeme, abyste si přezkontrolovali zdrojový kód všech aplikací a případně vyžádejte všechny nezávislé dodavatele softwaru (ISV) nebo poskytovatele aplikací.</span><span class="sxs-lookup"><span data-stu-id="a6292-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="a6292-123">Podpora Microsoftu vám taky poskytne seznam všech aplikací ADAL, které nejsou od Microsoftu, ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="a6292-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="a6292-124">**Migrace grafu AAD**</span><span class="sxs-lookup"><span data-stu-id="a6292-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="a6292-125">U aplikací, které používají diagram AAD, postupujte podle pokynů k migraci aplikací grafu AAD do Microsoft graphu:</span><span class="sxs-lookup"><span data-stu-id="a6292-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="a6292-126">[Naše kontrolní seznam migrace představuje bod Začínáme](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="a6292-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="a6292-127">Portál registrace aplikací pro Azure zobrazuje, které aplikace používají graf AAD.</span><span class="sxs-lookup"><span data-stu-id="a6292-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="a6292-128">Doporučujeme, abyste zkontrolovali všechny zdrojové kódy aplikací a případně Nezávislí poskytovatelé softwaru (ISV) nebo poskytovatelů aplikací.</span><span class="sxs-lookup"><span data-stu-id="a6292-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="a6292-129">Microsoft Support vám může také poskytnout informace o využití grafu AAD ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="a6292-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







