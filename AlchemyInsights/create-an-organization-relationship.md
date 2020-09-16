---
title: Vytvořením vztahu organizace umožníte uživatelům spolupracovat s jinou organizací.
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
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712726"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="131b8-102">Vytvořením vztahu organizace umožníte uživatelům spolupracovat s jinou organizací.</span><span class="sxs-lookup"><span data-stu-id="131b8-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="131b8-103">Na řídicím panelu centra pro správu Microsoft 365 přejděte na Exchange pro **správu**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="131b8-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="131b8-104">Přejděte na **organization**  >  **sdílení**organizace.</span><span class="sxs-lookup"><span data-stu-id="131b8-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="131b8-105">V části **sdílení organizace**klikněte na **Nový** .</span><span class="sxs-lookup"><span data-stu-id="131b8-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="131b8-106">V části **nový vztah organizace**zadejte do pole **název relace** popisný název pro vztah organizace.</span><span class="sxs-lookup"><span data-stu-id="131b8-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="131b8-107">Do pole **domény ke sdílení** zadejte doménu pro externí organizaci Office 365 nebo pro místní organizaci, které chcete, aby se zobrazily vaše kalendáře.</span><span class="sxs-lookup"><span data-stu-id="131b8-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="131b8-108">Pokud potřebujete zadat víc než jednu doménu, oddělte názvy domén čárkou.</span><span class="sxs-lookup"><span data-stu-id="131b8-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="131b8-109">Například contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="131b8-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="131b8-110">Zaškrtnutím políčka **Povolit sdílení informací o volném čase v kalendáři** Zapněte sdílení kalendáře s uvedenými doménami.</span><span class="sxs-lookup"><span data-stu-id="131b8-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="131b8-111">Nastavení úrovně sdílení informací o volném čase v kalendáři a nastavení uživatelů, kteří můžou sdílet informace o volném čase v kalendáři.</span><span class="sxs-lookup"><span data-stu-id="131b8-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="131b8-112">Pokud chcete nastavit úroveň přístupu k informacím o volném čase, vyberte jednu z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="131b8-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="131b8-113">**Informace o volném čase v kalendáři jenom s uvedením času**</span><span class="sxs-lookup"><span data-stu-id="131b8-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="131b8-114">**Informace o volném čase v kalendáři, předmět a místo konání**</span><span class="sxs-lookup"><span data-stu-id="131b8-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="131b8-115">Pokud chcete nastavit, kteří uživatelé budou sdílet informace o volném čase v kalendáři, vyberte jednu z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="131b8-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="131b8-116">**Všichni v organizaci**</span><span class="sxs-lookup"><span data-stu-id="131b8-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="131b8-117">**Zadaná skupina zabezpečení**</span><span class="sxs-lookup"><span data-stu-id="131b8-117">**A specified security group**</span></span>  

<span data-ttu-id="131b8-118">Kliknutím na **Procházet** vyberte skupinu zabezpečení ze seznamu a klikněte na **OK**.</span><span class="sxs-lookup"><span data-stu-id="131b8-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="131b8-119">Kliknutím na **Uložit** vytvořte vztah organizace.</span><span class="sxs-lookup"><span data-stu-id="131b8-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="131b8-120">**Poznámka:** Konfigurace křížových klientů nepodporují osobní kontakty pro vyhledávání informací o volném čase.</span><span class="sxs-lookup"><span data-stu-id="131b8-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="131b8-121">Pokud chcete, aby vyhledávání informací o volném čase fungovalo, musí být v globálním seznamu adres zahrnuté kontakty.</span><span class="sxs-lookup"><span data-stu-id="131b8-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="131b8-122">**Úplný výklad tohoto tématu najdete zde:**</span><span class="sxs-lookup"><span data-stu-id="131b8-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="131b8-123">Vytvoření vztahu organizace v Exchangi Online</span><span class="sxs-lookup"><span data-stu-id="131b8-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="131b8-124">Změna vztahů organizace v Exchangi Online</span><span class="sxs-lookup"><span data-stu-id="131b8-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="131b8-125">Odebrání vztahu organizace v Exchangi Online</span><span class="sxs-lookup"><span data-stu-id="131b8-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
