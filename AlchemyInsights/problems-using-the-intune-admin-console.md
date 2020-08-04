---
title: Problémy s používáním konzole pro správu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554880"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="c125d-102">Problémy s používáním konzole pro správu Intune</span><span class="sxs-lookup"><span data-stu-id="c125d-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="c125d-103">**"Přístup byl odepřen" při navigaci na portálu pro správu Intune.**</span><span class="sxs-lookup"><span data-stu-id="c125d-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="c125d-104">Pokud jste členem vlastní role Intune, ujistěte se, že je k vašemu účtu přiřazena licence Intune nebo Enterprise Mobility Suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="c125d-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="c125d-105">Pokud ke správě zařízení používáte nástroj Configuration Manager, ověřte, zda nejste součástí kolekce uživatelů Intune pro nástroj CONFIGURATION Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="c125d-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="c125d-106">Ověřte, zda vám byla v okně rolí Intune přiřazena příslušná oprávnění řízení správy (RBAC) založené na rolích.</span><span class="sxs-lookup"><span data-stu-id="c125d-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="c125d-107">Ověřte, zda použitá skupina není distribuční seznam.</span><span class="sxs-lookup"><span data-stu-id="c125d-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="c125d-108">Intune na portálu Azure podporuje jenom uživatelské účty, které patří do skupin zabezpečení Služby Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c125d-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="c125d-109">Zkontrolujte své skupiny v > **skupinách Azure**Portal nebo v Azure Portal > Azure Active  >  **Groups** **Directory**.</span><span class="sxs-lookup"><span data-stu-id="c125d-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="c125d-110">**Uživatel má příliš mnoho oprávnění pro přiřazenou roli Intune**</span><span class="sxs-lookup"><span data-stu-id="c125d-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="c125d-111">Poradit uživateli, **Intune**aby šel do rolí  >  **Intune Intune**  >  **Moje oprávnění**  >  **Exportovat** ke kontrole udělených oprávnění.</span><span class="sxs-lookup"><span data-stu-id="c125d-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="c125d-112">**Do role byla přidána skupina oboru, ale uživatelům v této roli se stále zobrazují ostatní uživatelé nebo zařízení**</span><span class="sxs-lookup"><span data-stu-id="c125d-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="c125d-113">Skupiny oborů neodfiltrují uživatele ani zařízení.</span><span class="sxs-lookup"><span data-stu-id="c125d-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="c125d-114">Skupiny oborů:</span><span class="sxs-lookup"><span data-stu-id="c125d-114">Scope groups:</span></span>

- <span data-ttu-id="c125d-115">Omezte, komu mohou uživatelé přiřazovat zásady nebo aplikace.</span><span class="sxs-lookup"><span data-stu-id="c125d-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="c125d-116">Povolit pouze určitým uživatelům spouštět vzdálené úlohy na zařízeních.</span><span class="sxs-lookup"><span data-stu-id="c125d-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="c125d-117">Další informace o skupinách oborů najdete v [tématu Řízení přístupu na základě rolí (RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="c125d-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="c125d-118">**Přidal(a) jsem uživatele do role Intune, ale pořád má plný přístup ke konzole pro správu Intune.**</span><span class="sxs-lookup"><span data-stu-id="c125d-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="c125d-119">Přejděte na Intune > **Users** na webu Azure Portal a ověřte, že uživatel není přiřazený k žádné z následujících rolí na webu Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="c125d-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="c125d-120">Globální správce</span><span class="sxs-lookup"><span data-stu-id="c125d-120">Global administrator</span></span>
- <span data-ttu-id="c125d-121">Správce služby Intune</span><span class="sxs-lookup"><span data-stu-id="c125d-121">Intune service administrator</span></span>
- <span data-ttu-id="c125d-122">Správce SharePointu</span><span class="sxs-lookup"><span data-stu-id="c125d-122">SharePoint administrator</span></span>

<span data-ttu-id="c125d-123">Další informace najdete v [tématu Řízení přístupu na základě rolí (RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="c125d-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="c125d-124">**Problémy s přístupem**</span><span class="sxs-lookup"><span data-stu-id="c125d-124">**Access Issues**</span></span>

<span data-ttu-id="c125d-125">Další informace najdete [v tématu Nemůžete se přihlásit k Office 365, Azure nebo Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="c125d-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>