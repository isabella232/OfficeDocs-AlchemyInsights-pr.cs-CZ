---
title: Jak přidat a spravovat správce – MCA FL/CL
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
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692013"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="387e8-102">Jak přidat a spravovat správce – MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="387e8-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="387e8-103">Pokud chcete fakturační účet spravovat pro smlouvu o zákaznících Microsoftu (MCA), můžete použít různé role s požadovanou úrovní přístupu.</span><span class="sxs-lookup"><span data-stu-id="387e8-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="387e8-104">Tyto role jsou kromě předdefinovaných rolí služby Azure, které vám pomůžou s kontrolou vašich zdrojů.</span><span class="sxs-lookup"><span data-stu-id="387e8-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="387e8-105">**Přidání fakturačních rolí na portálu Azure:**</span><span class="sxs-lookup"><span data-stu-id="387e8-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="387e8-106">Přihlaste se k [portálu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="387e8-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="387e8-107">Vyhledejte *správu nákladů + fakturace*.</span><span class="sxs-lookup"><span data-stu-id="387e8-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="387e8-108">Vyberte řízení přístupu (IAM) v oboru, jako je fakturační účet, Fakturační profil nebo faktura, kde chcete udělit přístup.</span><span class="sxs-lookup"><span data-stu-id="387e8-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="387e8-109">Na stránce řízení přístupu (IAM) se zobrazuje seznam uživatelů a skupin přiřazených k jednotlivým rolím daného oboru.</span><span class="sxs-lookup"><span data-stu-id="387e8-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="387e8-110">Pokud chcete uživateli udělit přístup, vyberte v horní části stránky možnost **Přidat** .</span><span class="sxs-lookup"><span data-stu-id="387e8-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="387e8-111">V rozevíracím seznamu *role* vyberte roli.</span><span class="sxs-lookup"><span data-stu-id="387e8-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="387e8-112">Zadejte e-mailovou adresu uživatele, kterému chcete udělit přístup.</span><span class="sxs-lookup"><span data-stu-id="387e8-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="387e8-113">Kliknutím na **Uložit** roli přiřadíte.</span><span class="sxs-lookup"><span data-stu-id="387e8-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="387e8-114">Pokud chcete odebrat přístup pro uživatele, vyberte uživatele s přiřazením rolí, které chcete odebrat.</span><span class="sxs-lookup"><span data-stu-id="387e8-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="387e8-115">Vyberte **Odebrat**.</span><span class="sxs-lookup"><span data-stu-id="387e8-115">Select **Remove**.</span></span>

<span data-ttu-id="387e8-116">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="387e8-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="387e8-117">Definice rolí fakturace</span><span class="sxs-lookup"><span data-stu-id="387e8-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="387e8-118">Role a úkoly fakturačního účtu</span><span class="sxs-lookup"><span data-stu-id="387e8-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="387e8-119">Začínáme s fakturačním účtem MCA</span><span class="sxs-lookup"><span data-stu-id="387e8-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="387e8-120">Kontrola přístupu ke Smlouvě o zákaznících Microsoftu</span><span class="sxs-lookup"><span data-stu-id="387e8-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
