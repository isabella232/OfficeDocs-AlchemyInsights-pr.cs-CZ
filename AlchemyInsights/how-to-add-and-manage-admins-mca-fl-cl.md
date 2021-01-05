---
title: Přidání a Správa správců
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755432"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="63833-102">Přidání a Správa správců</span><span class="sxs-lookup"><span data-stu-id="63833-102">How to add and manage admins</span></span>

<span data-ttu-id="63833-103">Na základě popisu problému jsme našli řešení.</span><span class="sxs-lookup"><span data-stu-id="63833-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="63833-104">Většina zákazníků dokázala svůj problém vyřešit vlastními po vás od naší dokumentace.</span><span class="sxs-lookup"><span data-stu-id="63833-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="63833-105">Pokud chcete fakturační účet spravovat pro smlouvu o zákaznících Microsoftu (MCA), můžete použít různé role s požadovanou úrovní přístupu.</span><span class="sxs-lookup"><span data-stu-id="63833-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="63833-106">Tyto role jsou kromě předdefinovaných rolí služby Azure, které vám pomůžou s kontrolou vašich zdrojů.</span><span class="sxs-lookup"><span data-stu-id="63833-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="63833-107">**Přidání fakturačních rolí na portálu Azure:**</span><span class="sxs-lookup"><span data-stu-id="63833-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="63833-108">Přihlaste se k [portálu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="63833-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="63833-109">Vyhledejte *správu nákladů + fakturace*.</span><span class="sxs-lookup"><span data-stu-id="63833-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="63833-110">Vyberte řízení přístupu (IAM) v oboru, jako je fakturační účet, Fakturační profil nebo faktura, kde chcete udělit přístup.</span><span class="sxs-lookup"><span data-stu-id="63833-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="63833-111">Na stránce řízení přístupu (IAM) se zobrazuje seznam uživatelů a skupin přiřazených k jednotlivým rolím daného oboru.</span><span class="sxs-lookup"><span data-stu-id="63833-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="63833-112">Pokud chcete uživateli udělit přístup, vyberte v horní části stránky možnost **Přidat** .</span><span class="sxs-lookup"><span data-stu-id="63833-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="63833-113">V rozevíracím seznamu *role* vyberte roli.</span><span class="sxs-lookup"><span data-stu-id="63833-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="63833-114">Zadejte e-mailovou adresu uživatele, kterému chcete udělit přístup.</span><span class="sxs-lookup"><span data-stu-id="63833-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="63833-115">Kliknutím na **Uložit** roli přiřadíte.</span><span class="sxs-lookup"><span data-stu-id="63833-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="63833-116">Pokud chcete odebrat přístup pro uživatele, vyberte uživatele s přiřazením rolí, které chcete odebrat.</span><span class="sxs-lookup"><span data-stu-id="63833-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="63833-117">Vyberte **Odebrat**.</span><span class="sxs-lookup"><span data-stu-id="63833-117">Select **Remove**.</span></span>

<span data-ttu-id="63833-118">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="63833-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="63833-119">Definice rolí fakturace</span><span class="sxs-lookup"><span data-stu-id="63833-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="63833-120">Role a úkoly fakturačního účtu</span><span class="sxs-lookup"><span data-stu-id="63833-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="63833-121">Začínáme s fakturačním účtem MCA</span><span class="sxs-lookup"><span data-stu-id="63833-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="63833-122">Kontrola přístupu ke Smlouvě o zákaznících Microsoftu</span><span class="sxs-lookup"><span data-stu-id="63833-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
