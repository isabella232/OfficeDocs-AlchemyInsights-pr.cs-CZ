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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923124"
---
# <a name="rbac-rules"></a>Pravidla RBAC

Pokud se zobrazí chyba oprávnění: 

- Klient s ID objektu nemá oprávnění k provádění akcí nad **oborem (kód: AuthorizationFailed):** Při pokusu o vytvoření zdroje zkontrolujte, jestli jste aktuálně přihlášení k uživateli, který má přiřazenou roli, která má oprávnění k zápisu k prostředku ve vybraném oboru. Pokud třeba chcete spravovat virtuální počítače ve skupině [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) prostředků, měli byste mít roli Přispěvatel virtuálního počítače ve skupině prostředků (nebo nadřazeném oboru). Seznam oprávnění pro jednotlivé předdefinované role najdete v tématu Předdefinované [role pro prostředky Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Nemáte oprávnění k vytvoření žádosti o **podporu:** Když se pokusíte vytvořit nebo aktualizovat lístek podpory, zkontrolujte, jestli jste aktuálně přihlášení k uživateli, který má přiřazenou roli, která má oprávnění Microsoft.Support/supportTickets/write, například Přispěvatel žádosti o [podporu.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Nelze vytvořit žádná další přiřazení rolí **(kód: RoleAssignmentLimitExceeded):** Když se pokusíte přiřadit roli, zkuste místo toho snížit počet přiřazení rolí přiřazením rolí skupinám. Azure podporuje až **2 000** přiřazení rolí na jedno předplatné.

Další podrobnosti o rolích Azure RBAC najdete v [tématu Role Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
