---
title: Řešení potíží s SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429472"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="b15d8-102">Řešení potíží s SSPR</span><span class="sxs-lookup"><span data-stu-id="b15d8-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="b15d8-103">**Mám problémy s konfigurací resetování hesla**</span><span class="sxs-lookup"><span data-stu-id="b15d8-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="b15d8-104">Pokud jste správce a hledáte, jak povolit samoobslužné resetování hesla, podívejte se, jak v organizaci nakonfigurovat resetování hesla pomocí funkce Kurz povolte nástroj [SSPR.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)</span><span class="sxs-lookup"><span data-stu-id="b15d8-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="b15d8-105">Možná si taky budete chtít prohlédněte licenční [požadavky.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b15d8-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="b15d8-106">Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.</span><span class="sxs-lookup"><span data-stu-id="b15d8-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="b15d8-107">**Jenom cloudové uživatele** – všechny placené SKU Office 365 (O365) nebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="b15d8-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="b15d8-108">**Cloudové a místní** uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="b15d8-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="b15d8-109">Další informace o samoobslužných resetování hesel najdete v [častých otázkách.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b15d8-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="b15d8-110">**Zobrazí se mi chybová zpráva**</span><span class="sxs-lookup"><span data-stu-id="b15d8-110">**I'm getting an error message**</span></span>

<span data-ttu-id="b15d8-111">V tomto článku najdete informace o běžných chybách a jejich řešeních: [Řešení samoobslužných resetování hesel](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b15d8-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="b15d8-112">**Mám problém se zásadou pro resetování hesla**</span><span class="sxs-lookup"><span data-stu-id="b15d8-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="b15d8-113">Pokud se vaše zásada resetování hesla nechová podle očekávání nebo máte dotazy k zásadám resetování hesla, projděte si tento článek: Zásady hesel a omezení v [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b15d8-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="b15d8-114">Zásady pro resetování hesel se nevztahují na správce.</span><span class="sxs-lookup"><span data-stu-id="b15d8-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="b15d8-115">Microsoft vynucuje silné výchozí zásady resetování hesla ve dvou bránách pro libovolnou roli správce Azure.</span><span class="sxs-lookup"><span data-stu-id="b15d8-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="b15d8-116">Ujistěte se, že testujete s uživatelem, který není správcem.</span><span class="sxs-lookup"><span data-stu-id="b15d8-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="b15d8-117">Další informace o resetování zásad správce najdete v tomto článku: Rozdíly [v zásadách resetování správcem.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="b15d8-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="b15d8-118">**Nechci, aby uživatelé zaregistroval další bezpečnostní údaje pro resetování hesla.**</span><span class="sxs-lookup"><span data-stu-id="b15d8-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="b15d8-119">Data (atributy e-mailu a telefonu) pro uživatele můžete předem vyplnit pomocí rozhraní API, PowerShellu nebo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b15d8-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="b15d8-120">Jak na to:</span><span class="sxs-lookup"><span data-stu-id="b15d8-120">To learn how read:</span></span>

- [<span data-ttu-id="b15d8-121">Nasazení resetování hesla bez nutnosti registrace uživatelů</span><span class="sxs-lookup"><span data-stu-id="b15d8-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="b15d8-122">Jaká data se používají při resetování hesla</span><span class="sxs-lookup"><span data-stu-id="b15d8-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="b15d8-123">**Chci, aby si uživatelé zaregistroval(a) další bezpečnostní údaje pro resetování hesla.**</span><span class="sxs-lookup"><span data-stu-id="b15d8-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="b15d8-124">Vemte uživatele, aby si zaregistrovali svoje bezpečnostní údaje k samoobslužnému resetování hesla tak, že je nasměrujete [na aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)</span><span class="sxs-lookup"><span data-stu-id="b15d8-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="b15d8-125">Po naplnění dat uživatelem (uživatelem nebo správcem) nasměrujte [](https://passwordreset.microsoftonline.com/) uživatele na správce, aby aka.ms/sspr aby mohli uživatelé obnovovat svá vlastní hesla.</span><span class="sxs-lookup"><span data-stu-id="b15d8-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="b15d8-126">Pokud se u uživatelů pořád dochází k problémům, jsou s největší pravděpodobností **federovaní** nebo synchronizovaní uživatelé **s hodnotou hash** hesel.</span><span class="sxs-lookup"><span data-stu-id="b15d8-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="b15d8-127">To znamená, že může být nějaký problém se službou zpětného zápisu hesel.</span><span class="sxs-lookup"><span data-stu-id="b15d8-127">This means there is likely a problem with the Password Writeback service.</span></span>