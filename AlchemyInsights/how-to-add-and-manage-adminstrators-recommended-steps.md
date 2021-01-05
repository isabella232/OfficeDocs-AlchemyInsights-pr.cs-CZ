---
title: Přidání a Správa správců – doporučené kroky
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755828"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="a1915-102">Přidání a Správa správců – doporučené kroky</span><span class="sxs-lookup"><span data-stu-id="a1915-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="a1915-103">Na základě popisu problému jsme našli řešení.</span><span class="sxs-lookup"><span data-stu-id="a1915-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="a1915-104">Většina zákazníků dokázala svůj problém vyřešit vlastními po vás od naší dokumentace.</span><span class="sxs-lookup"><span data-stu-id="a1915-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="a1915-105">**Úprava Správce předplatného nebo spolusprávce**</span><span class="sxs-lookup"><span data-stu-id="a1915-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="a1915-106">Správce účtu může upravovat obě role, zatímco Správce předplatného může změnit jenom spolusprávce na [portálu Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="a1915-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="a1915-107">Přidání nebo změna správců předplatného Azure</span><span class="sxs-lookup"><span data-stu-id="a1915-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="a1915-108">**Aktualizace předplatného správce nebo Co-Administrator pro interní (AIRS) předplatná**</span><span class="sxs-lookup"><span data-stu-id="a1915-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="a1915-109">Správce služby nebo spolusprávce může tuto akci sám využít následujícími kroky:</span><span class="sxs-lookup"><span data-stu-id="a1915-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="a1915-110">Přihlaste se k [portálu Azure](https://ms.portal.azure.com/#home) a v levém okně klikněte na **Správa nákladů + fakturace** .</span><span class="sxs-lookup"><span data-stu-id="a1915-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="a1915-111">Klikněte na položku řádku s předplatným.</span><span class="sxs-lookup"><span data-stu-id="a1915-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="a1915-112">Otevře se přehled předplatného.</span><span class="sxs-lookup"><span data-stu-id="a1915-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="a1915-113">V okně  předplatná klikněte na **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="a1915-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="a1915-114">Klikněte na tlačítko **Správce služby** .</span><span class="sxs-lookup"><span data-stu-id="a1915-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="a1915-115">Zadejte e-mail uživatele, kterého chcete nastavit jako správce služby, a klikněte na **OK**.</span><span class="sxs-lookup"><span data-stu-id="a1915-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="a1915-116">**Přidání, změna nebo odebrání spolusprávce**</span><span class="sxs-lookup"><span data-stu-id="a1915-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="a1915-117">Přihlaste se k [portálu Azure](https://ms.portal.azure.com/#home) jako správce služby.</span><span class="sxs-lookup"><span data-stu-id="a1915-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="a1915-118">Otevřete [předplatná](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) a vyberte předplatné.</span><span class="sxs-lookup"><span data-stu-id="a1915-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="a1915-119">(Spolusprávce lze přiřadit pouze v oboru předplatného.)</span><span class="sxs-lookup"><span data-stu-id="a1915-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="a1915-120">Přechod na **ovládací panel pro správu Accessu (IAM)**  >  **klasické správce**  >  **přidá**  >  možnost **Přidat spolusprávce** , aby otevřela podokno **Přidat** spolusprávce (Pokud je možnost Přidat spolusprávce zakázaná).</span><span class="sxs-lookup"><span data-stu-id="a1915-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="a1915-121">Vyberte uživatele, kterého chcete přidat, a klikněte na **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="a1915-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="a1915-122">**Víc se uč:**</span><span class="sxs-lookup"><span data-stu-id="a1915-122">**Learn more:**</span></span>
- [<span data-ttu-id="a1915-123">Přidání spolusprávce</span><span class="sxs-lookup"><span data-stu-id="a1915-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a1915-124">Odebrání spolusprávce</span><span class="sxs-lookup"><span data-stu-id="a1915-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a1915-125">Změna správce služeb</span><span class="sxs-lookup"><span data-stu-id="a1915-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a1915-126">Zobrazení správce účtu</span><span class="sxs-lookup"><span data-stu-id="a1915-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a1915-127">Správa Accessu pomocí RBAC a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="a1915-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="a1915-128">**Přidání nebo odebrání uživatelů pomocí služby Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="a1915-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="a1915-129">Do služby Azure Active Directory (Azure AD) můžete přidat nové uživatele nebo odstranit stávající uživatele:</span><span class="sxs-lookup"><span data-stu-id="a1915-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="a1915-130">Pokud chcete přidat nového uživatele, přihlaste se k [portálu Azure](https://ms.portal.azure.com/#home) jako správce uživatelů pro organizaci.</span><span class="sxs-lookup"><span data-stu-id="a1915-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="a1915-131">Vyberte **Azure Active Directory**, vyberte **Uživatelé** a klikněte na **Nový uživatel**.</span><span class="sxs-lookup"><span data-stu-id="a1915-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="a1915-132">Na stránce **uživatel** vyplňte požadované informace.</span><span class="sxs-lookup"><span data-stu-id="a1915-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="a1915-133">Klikněte na **vytvořit**.</span><span class="sxs-lookup"><span data-stu-id="a1915-133">Click **Create**.</span></span> <span data-ttu-id="a1915-134">Uživatel se vytvoří a přidá do tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a1915-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="a1915-135">**Další informace**:</span><span class="sxs-lookup"><span data-stu-id="a1915-135">**Learn more**:</span></span>

- [<span data-ttu-id="a1915-136">Přidání nového uživatele</span><span class="sxs-lookup"><span data-stu-id="a1915-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="a1915-137">Odstranění uživatele</span><span class="sxs-lookup"><span data-stu-id="a1915-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="a1915-138">Přidání nebo aktualizace informací o profilu uživatele pomocí služby Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a1915-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="a1915-139">**Doporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="a1915-139">**Recommended documents**</span></span>

- [<span data-ttu-id="a1915-140">Co je řízení přístupu založené na rolích (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="a1915-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="a1915-141">Pochopení různých rolí v Azure</span><span class="sxs-lookup"><span data-stu-id="a1915-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="a1915-142">Oprávnění role správce v Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a1915-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="a1915-143">Kurz: udělení přístupu pro uživatele pomocí RBAC a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="a1915-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="a1915-144">Řešení problémů v Azure</span><span class="sxs-lookup"><span data-stu-id="a1915-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="a1915-145">Uspořádání zdrojů do skupin Azure Management</span><span class="sxs-lookup"><span data-stu-id="a1915-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="a1915-146">Jak požádat o kopii faktury Azure e-mailem</span><span class="sxs-lookup"><span data-stu-id="a1915-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="a1915-147">Jak přidat, aktualizovat nebo odebrat kredit nebo debetní kartu z Azure</span><span class="sxs-lookup"><span data-stu-id="a1915-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="a1915-148">Správa předplatného (opětovné aktivace/zrušení/přepnutí)</span><span class="sxs-lookup"><span data-stu-id="a1915-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



