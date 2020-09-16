---
title: Problémy s používáním konzoly pro správu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728280"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="c01ac-102">Problémy s používáním konzoly pro správu Intune</span><span class="sxs-lookup"><span data-stu-id="c01ac-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="c01ac-103">**Při navigaci na portálu pro správu Intune se zobrazí zpráva Access denied (přístup odepřen).**</span><span class="sxs-lookup"><span data-stu-id="c01ac-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="c01ac-104">Pokud jste členem vlastní role Intune, ujistěte se, že k vašemu účtu je přiřazená licence EMS (Intune nebo Enterprise mobility).</span><span class="sxs-lookup"><span data-stu-id="c01ac-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="c01ac-105">Pokud ke správě zařízení používáte nástroj Configuration Manager, ověřte, že nejste součástí Intune User Collection pro MDM Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="c01ac-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="c01ac-106">Zkontrolujte, jestli máte v okně role Intune přiřazená oprávnění řízení správy založené na rolích (RBAC).</span><span class="sxs-lookup"><span data-stu-id="c01ac-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="c01ac-107">Ověřte, že použitá skupina není distribuční seznam.</span><span class="sxs-lookup"><span data-stu-id="c01ac-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="c01ac-108">Intune na Azure Portal podporuje jenom uživatelské účty patřící do skupin zabezpečení Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c01ac-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="c01ac-109">Prohlédněte si skupiny v Azure Portalu > skupiny **Intune**  >  **Groups**nebo v Azure Portal > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="c01ac-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="c01ac-110">**Uživatel má příliš mnoho oprávnění k přiřazené roli Intune.**</span><span class="sxs-lookup"><span data-stu-id="c01ac-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="c01ac-111">Informujte uživatele, aby přešel na **Intune**  >  **Intune roles**Intune  >  **My permissions**  >  **Export**</span><span class="sxs-lookup"><span data-stu-id="c01ac-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="c01ac-112">**Do role přidal (a) skupinu oborů, ale uživatelé v dané roli pořád uvidí další uživatele nebo zařízení.**</span><span class="sxs-lookup"><span data-stu-id="c01ac-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="c01ac-113">Skupiny oborů nefiltrují uživatele nebo zařízení.</span><span class="sxs-lookup"><span data-stu-id="c01ac-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="c01ac-114">Skupiny oborů:</span><span class="sxs-lookup"><span data-stu-id="c01ac-114">Scope groups:</span></span>

- <span data-ttu-id="c01ac-115">Omezte počet uživatelů, kteří můžou přiřazovat zásady nebo aplikace.</span><span class="sxs-lookup"><span data-stu-id="c01ac-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="c01ac-116">Povolte spouštění vzdálených úloh na zařízeních pouze konkrétním uživatelům.</span><span class="sxs-lookup"><span data-stu-id="c01ac-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="c01ac-117">Další informace o skupinách oborů najdete v tématu  [řízení přístupu založeném na rolích (RBAC) v Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="c01ac-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="c01ac-118">**Do role Intune jsem přidal (a), ale pořád má úplný přístup ke konzole správce Intune.**</span><span class="sxs-lookup"><span data-stu-id="c01ac-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="c01ac-119">Přejděte na Intune > **uživatele** na portálu Azure a ověřte, jestli uživatel nemá přiřazenou žádnou z následujících rolí na portálu Azure:</span><span class="sxs-lookup"><span data-stu-id="c01ac-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="c01ac-120">Globální správce</span><span class="sxs-lookup"><span data-stu-id="c01ac-120">Global administrator</span></span>
- <span data-ttu-id="c01ac-121">Intune – Správce služby</span><span class="sxs-lookup"><span data-stu-id="c01ac-121">Intune service administrator</span></span>
- <span data-ttu-id="c01ac-122">Správce SharePointu</span><span class="sxs-lookup"><span data-stu-id="c01ac-122">SharePoint administrator</span></span>

<span data-ttu-id="c01ac-123">Další informace najdete v tématu [řízení přístupu založeném na rolích (RBAC) v Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="c01ac-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="c01ac-124">**Problémy s přístupem**</span><span class="sxs-lookup"><span data-stu-id="c01ac-124">**Access Issues**</span></span>

<span data-ttu-id="c01ac-125">Další informace najdete v článku [nemůžete se přihlásit k Office 365, Azure nebo Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="c01ac-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>