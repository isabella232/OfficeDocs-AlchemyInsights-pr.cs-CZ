---
title: 'Role RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583351"
---
# <a name="rbac-rules"></a><span data-ttu-id="58eb7-102">Pravidla RBAC</span><span class="sxs-lookup"><span data-stu-id="58eb7-102">RBAC rules</span></span>

<span data-ttu-id="58eb7-103">Pokud se zobrazí chyba oprávnění:</span><span class="sxs-lookup"><span data-stu-id="58eb7-103">If you get the permission error:</span></span> 

- <span data-ttu-id="58eb7-104">**Klient s ID objektu nemá oprávnění provádět akce nad oborem (kód: AuthorizationFailed)**: když se pokusíte vytvořit prostředek, zkontrolujte, že jste aktuálně přihlášení s uživatelem, kterému je přiřazená role s oprávněním k zápisu pro prostředek ve vybraném oboru.</span><span class="sxs-lookup"><span data-stu-id="58eb7-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="58eb7-105">Chcete-li například spravovat virtuální počítače ve skupině prostředků, měli byste mít roli [Přispěvatel virtuálního počítače](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) ve skupině zdrojů (nebo na nadřazeném oboru).</span><span class="sxs-lookup"><span data-stu-id="58eb7-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="58eb7-106">Seznam oprávnění pro každou předdefinovanou roli najdete v tématu [předdefinované role pro prostředky Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="58eb7-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="58eb7-107">Nemáte **oprávnění k vytvoření žádosti o podporu**: když se pokusíte vytvořit nebo aktualizovat lístek podpory, zkontrolujte, jestli jste přihlášení pomocí uživatele, kterému je přiřazená role s oprávněním Microsoft. support/supportTickets/Write, třeba [Přispěvatel žádostí o podporu](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="58eb7-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="58eb7-108">Nelze **vytvořit další přiřazení rolí (kód: RoleAssignmentLimitExceeded)**: když se pokusíte přiřadit roli, zkuste snížit počet přiřazení rolí přiřazením rolí skupinám.</span><span class="sxs-lookup"><span data-stu-id="58eb7-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="58eb7-109">Azure podporuje až **2000** přiřazení rolí na předplatné.</span><span class="sxs-lookup"><span data-stu-id="58eb7-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="58eb7-110">Další informace o rolích Azure RBAC najdete v tématu [role služby Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="58eb7-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
