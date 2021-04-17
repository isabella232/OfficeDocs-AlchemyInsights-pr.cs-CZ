---
title: Vytvoření relace organizace, která uživatelům umožní spolupracovat s jinou organizací
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816121"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="6de50-102">Vytvoření relace organizace, která uživatelům umožní spolupracovat s jinou organizací</span><span class="sxs-lookup"><span data-stu-id="6de50-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="6de50-103">Na řídicím panelu Centra pro správu Microsoftu 365 přejděte na **Správce**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="6de50-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="6de50-104">Přejděte na **sdílení**  >  **organizace**.</span><span class="sxs-lookup"><span data-stu-id="6de50-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="6de50-105">V **části Sdílení organizace** klikněte na **Nový** .</span><span class="sxs-lookup"><span data-stu-id="6de50-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="6de50-106">V **novém vztahu organizace** zadejte do pole Název **relace** popisný název relace organizace.</span><span class="sxs-lookup"><span data-stu-id="6de50-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="6de50-107">Do pole **Domény** ke sdílení s zadejte doménu pro externí místní organizaci Office 365 nebo Exchange, kterou chcete nechat zobrazit kalendáře.</span><span class="sxs-lookup"><span data-stu-id="6de50-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="6de50-108">Pokud potřebujete zadat víc než jednu doménu, oddělte je čárkou.</span><span class="sxs-lookup"><span data-stu-id="6de50-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="6de50-109">Můžete třeba contoso.com service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="6de50-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="6de50-110">Pokud chcete **zapnout** sdílení kalendáře s doménami, které jste v seznamu měli, zaškrtněte políčko Povolit sdílení informací o volném čase v kalendáři.</span><span class="sxs-lookup"><span data-stu-id="6de50-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="6de50-111">Nastavte úroveň sdílení informací o volném čase v kalendáři a nastavte, kteří uživatelé mohou sdílet informace o volném čase v kalendáři.</span><span class="sxs-lookup"><span data-stu-id="6de50-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="6de50-112">Pokud chcete nastavit úroveň přístupu k volnému čase, vyberte jednu z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="6de50-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="6de50-113">**Informace o volném čase v kalendáři jenom s uvedením času**</span><span class="sxs-lookup"><span data-stu-id="6de50-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="6de50-114">**Informace o volném čase, předmětu a místě v kalendáři**</span><span class="sxs-lookup"><span data-stu-id="6de50-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="6de50-115">Pokud chcete nastavit, kteří uživatelé budou sdílet informace o volném čase v kalendáři, vyberte jednu z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="6de50-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="6de50-116">**Všichni ve vaší organizaci**</span><span class="sxs-lookup"><span data-stu-id="6de50-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="6de50-117">**Zadaná skupina zabezpečení**</span><span class="sxs-lookup"><span data-stu-id="6de50-117">**A specified security group**</span></span>  

<span data-ttu-id="6de50-118">Kliknutím **na** procházet vyberte skupinu zabezpečení ze seznamu a klikněte na **OK.**</span><span class="sxs-lookup"><span data-stu-id="6de50-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="6de50-119">Pokud **chcete vytvořit** relaci organizace, klikněte na Uložit.</span><span class="sxs-lookup"><span data-stu-id="6de50-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="6de50-120">**Poznámka:** Konfigurace mezi tenanty nepodporují osobní kontakty pro vyhledávání v volném čase.</span><span class="sxs-lookup"><span data-stu-id="6de50-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="6de50-121">Aby vyhledávání v volném čase fungovalo, musí být kontakty zahrnuté do globálního seznamu adres.</span><span class="sxs-lookup"><span data-stu-id="6de50-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="6de50-122">**Pokud chcete plně porozumět tomuto tématu, přečtěte si prosím:**</span><span class="sxs-lookup"><span data-stu-id="6de50-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="6de50-123">Vytvoření relace organizace v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6de50-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="6de50-124">Změna relace organizace v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6de50-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="6de50-125">Odebrání relace organizace v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6de50-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
