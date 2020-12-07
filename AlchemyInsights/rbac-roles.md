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
# <a name="rbac-rules"></a>Pravidla RBAC

Pokud se zobrazí chyba oprávnění: 

- **Klient s ID objektu nemá oprávnění provádět akce nad oborem (kód: AuthorizationFailed)**: když se pokusíte vytvořit prostředek, zkontrolujte, že jste aktuálně přihlášení s uživatelem, kterému je přiřazená role s oprávněním k zápisu pro prostředek ve vybraném oboru. Chcete-li například spravovat virtuální počítače ve skupině prostředků, měli byste mít roli [Přispěvatel virtuálního počítače](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) ve skupině zdrojů (nebo na nadřazeném oboru). Seznam oprávnění pro každou předdefinovanou roli najdete v tématu [předdefinované role pro prostředky Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Nemáte **oprávnění k vytvoření žádosti o podporu**: když se pokusíte vytvořit nebo aktualizovat lístek podpory, zkontrolujte, jestli jste přihlášení pomocí uživatele, kterému je přiřazená role s oprávněním Microsoft. support/supportTickets/Write, třeba [Přispěvatel žádostí o podporu](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Nelze **vytvořit další přiřazení rolí (kód: RoleAssignmentLimitExceeded)**: když se pokusíte přiřadit roli, zkuste snížit počet přiřazení rolí přiřazením rolí skupinám. Azure podporuje až **2000** přiřazení rolí na předplatné.

Další informace o rolích Azure RBAC najdete v tématu [role služby Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
