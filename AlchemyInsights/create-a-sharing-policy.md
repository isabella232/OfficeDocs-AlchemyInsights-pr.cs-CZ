---
title: Vytvoření zásad sdílení umožňující uživatelům sdílet kalendář s lidmi mimo vaši organizaci
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
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816265"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="40ccb-102">Vytvoření zásad sdílení umožňující uživatelům sdílet kalendář s lidmi mimo vaši organizaci</span><span class="sxs-lookup"><span data-stu-id="40ccb-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="40ccb-103">Na řídicím panelu Centra pro správu Microsoft 365 přejděte na **Správce** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="40ccb-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="40ccb-104">Přejděte na **Organizace** > **Sdílení**.</span><span class="sxs-lookup"><span data-stu-id="40ccb-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="40ccb-105">V zobrazení seznamu klikněte v části **Sdílení s jednotlivci** na **Nové** .</span><span class="sxs-lookup"><span data-stu-id="40ccb-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="40ccb-106">V části **Nová zásada sdílení** zadejte popisný název zásady sdílení do pole **Název zásady**.</span><span class="sxs-lookup"><span data-stu-id="40ccb-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="40ccb-107">Klikněte na **Přidat** a definujte pravidla sdílení pro tuto zásadu.</span><span class="sxs-lookup"><span data-stu-id="40ccb-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="40ccb-108">V části **pravidlo sdílení** vyberte jednu z následujících možností pro určení domény, se kterou chcete soubory sdílet:</span><span class="sxs-lookup"><span data-stu-id="40ccb-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="40ccb-109">**Sdílení se všemi doménami**</span><span class="sxs-lookup"><span data-stu-id="40ccb-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="40ccb-110">**Sdílení s konkrétní doménou**</span><span class="sxs-lookup"><span data-stu-id="40ccb-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="40ccb-111">Pokud vyberete **Sdílení s konkrétní doménou**, zadejte název domény, se kterou chcete kalendář sdílet.</span><span class="sxs-lookup"><span data-stu-id="40ccb-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="40ccb-112">Pokud pro tuto zásadu sdílení potřebujete zadat víc než jednu doménu, uložte nastavení pro první doménu a pak upravte pravidla sdílení a přidejte další domény.</span><span class="sxs-lookup"><span data-stu-id="40ccb-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="40ccb-113">Pokud chcete upřesnit, které informace se mají sdílet, zaškrtněte políčko **Sdílet složku kalendáře** a pak vyberte jednu z následujících možností:</span><span class="sxs-lookup"><span data-stu-id="40ccb-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="40ccb-114">**Informace o volném čase v kalendáři jenom s uvedením času**</span><span class="sxs-lookup"><span data-stu-id="40ccb-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="40ccb-115">**Informace o volném čase v kalendáři s uvedením času, předmětu a místa**</span><span class="sxs-lookup"><span data-stu-id="40ccb-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="40ccb-116">**Všechny informace o událostech v kalendáři, včetně času, předmětu, místa a názvu**</span><span class="sxs-lookup"><span data-stu-id="40ccb-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="40ccb-117">Kliknutím na **uložit** nastavíte pravidla pro zásady sdílení.</span><span class="sxs-lookup"><span data-stu-id="40ccb-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="40ccb-118">Pokud chcete tyto zásady sdílení nastavit jako nové výchozí zásady sdílení pro všechny uživatele ve vaší organizaci, zaškrtněte políčko **Nastavit tuto zásadu jako moji výchozí zásadu sdílení**.</span><span class="sxs-lookup"><span data-stu-id="40ccb-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="40ccb-119">Zásady sdílení vytvoříte kliknutím na **uložit**.</span><span class="sxs-lookup"><span data-stu-id="40ccb-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="40ccb-120">**Pokud chcete plně porozumět tomuto tématu, přečtěte si prosím:**</span><span class="sxs-lookup"><span data-stu-id="40ccb-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="40ccb-121">Vytvoření zásad sdílení v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="40ccb-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="40ccb-122">Použití zásad sdílení u poštovních schránek v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="40ccb-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="40ccb-123">Úprava, zakázání a odstranění zásad sdílení v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="40ccb-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)