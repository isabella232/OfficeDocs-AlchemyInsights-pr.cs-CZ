---
title: Změna výchozí domény Yammeru
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 93c82b7e60838e0127062e8bf5ab394bb29650d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793859"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="ee20d-102">Změna výchozí/primární domény Yammeru</span><span class="sxs-lookup"><span data-stu-id="ee20d-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="ee20d-103">URL adresa Yammeru obsahuje aktuální název primární domény pro vaši síť Yammeru.</span><span class="sxs-lookup"><span data-stu-id="ee20d-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="ee20d-104">Název domény se nemusí shodovat s názvem primární domény nastaveným v Office 365 nebo v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee20d-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="ee20d-105">Chování se mění v závislosti na počtu vlastních domén přidaných do tenanta a na tom, jestli je Yammer v podporované konfiguraci (1 tenant na 1 síť, nebo 1:1).</span><span class="sxs-lookup"><span data-stu-id="ee20d-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="ee20d-106">K dispozici je dokumentace k [doménám Yammeru a Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).</span><span class="sxs-lookup"><span data-stu-id="ee20d-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="ee20d-107">Nejčastějším důvodem, proč vidíte nesprávnou doménu, je více sítí Yammeru, které je potřeba konsolidovat.</span><span class="sxs-lookup"><span data-stu-id="ee20d-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="ee20d-108">Prvním a důležitým krokem je [konsolidace na jedinou síť](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) prostřednictvím nástroje na migraci sítě.</span><span class="sxs-lookup"><span data-stu-id="ee20d-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="ee20d-109">To je potřeba dokončit, než budete nastavovat svou primární doménu.</span><span class="sxs-lookup"><span data-stu-id="ee20d-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="ee20d-110">**Žádné vlastní domény**</span><span class="sxs-lookup"><span data-stu-id="ee20d-110">**No custom domains**</span></span>

<span data-ttu-id="ee20d-111">U nových tenantů se pro Yammer použije výchozí doména (např. fabrikam.onmicrosoft.com) tenanta.</span><span class="sxs-lookup"><span data-stu-id="ee20d-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="ee20d-112">Primární doména je nastavená na yammer.com/fabrikam.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="ee20d-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="ee20d-113">**Jedna vlastní doména**</span><span class="sxs-lookup"><span data-stu-id="ee20d-113">**Single custom domain**</span></span>

<span data-ttu-id="ee20d-114">Yammer automaticky vybere vlastní doménu (např. fabrikam.com) tenanta a nastaví ji jako primární doménu Yammeru.</span><span class="sxs-lookup"><span data-stu-id="ee20d-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="ee20d-115">Je nastavená na yammer.com/fabrikam.com.</span><span class="sxs-lookup"><span data-stu-id="ee20d-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="ee20d-116">Tuto změnu provádí služba synchronizace domén a může trvat až 24 hodin, než se projeví.</span><span class="sxs-lookup"><span data-stu-id="ee20d-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="ee20d-117">**Více vlastních domén**</span><span class="sxs-lookup"><span data-stu-id="ee20d-117">**Multiple custom domains**</span></span>

<span data-ttu-id="ee20d-118">Yammeru může mít doménu, která se od výchozí domény tenanta liší.</span><span class="sxs-lookup"><span data-stu-id="ee20d-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="ee20d-119">Když existuje víc vlastních domén, Yammer se nebude pokoušet hádat, která z dostupných domén je ta správná.</span><span class="sxs-lookup"><span data-stu-id="ee20d-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="ee20d-120">Bude potřeba, abyste požádali o změnu názvu primární domény na vámi vybranou doménu.</span><span class="sxs-lookup"><span data-stu-id="ee20d-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="ee20d-121">**Další informace o řešení potíží**</span><span class="sxs-lookup"><span data-stu-id="ee20d-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="ee20d-122">V některých případech se mohly domény přesunout mezi tenanty a službu synchronizace domén se nemuselo povést úspěšně spustit.</span><span class="sxs-lookup"><span data-stu-id="ee20d-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="ee20d-123">Kromě nesprávné primární domény můžete mít potíže s přihlášením nebo jiné problémy.</span><span class="sxs-lookup"><span data-stu-id="ee20d-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="ee20d-124">Když to budete chtít vyřešit, možná bude potřeba domény přesunout na správnou síť s pomocí podpory Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="ee20d-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="ee20d-125">Taková situace vyžaduje přímou asistenci a může nějakou dobu trvat, než se vyřeší. Zvláště pak tehdy, když je seznam domén opravdu dlouhý.</span><span class="sxs-lookup"><span data-stu-id="ee20d-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="ee20d-126">Požádejte o asistenci s řešením podobných potíží.</span><span class="sxs-lookup"><span data-stu-id="ee20d-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="ee20d-127">Až budete spolupracovat se zástupcem podpory, ověří si, že je doména ověřená u tenanta, kterého spravujete vy.</span><span class="sxs-lookup"><span data-stu-id="ee20d-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="ee20d-128">Pokud máte domény přidané k tenantovi, ale neověřené prostřednictvím DNS, možná bude kvůli ověření potřeba dodat další informace.</span><span class="sxs-lookup"><span data-stu-id="ee20d-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="ee20d-129">Pokud chcete proces urychlit, ujistěte se, že jsou domény ověřené prostřednictvím DNS.</span><span class="sxs-lookup"><span data-stu-id="ee20d-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
