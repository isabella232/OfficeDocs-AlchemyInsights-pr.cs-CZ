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
# <a name="problems-using-the-intune-admin-console"></a>Problémy s používáním konzole pro správu Intune

**"Přístup byl odepřen" při navigaci na portálu pro správu Intune.**

- Pokud jste členem vlastní role Intune, ujistěte se, že je k vašemu účtu přiřazena licence Intune nebo Enterprise Mobility Suite (EMS).
- Pokud ke správě zařízení používáte nástroj Configuration Manager, ověřte, zda nejste součástí kolekce uživatelů Intune pro nástroj CONFIGURATION Manager MDM.
- Ověřte, zda vám byla v okně rolí Intune přiřazena příslušná oprávnění řízení správy (RBAC) založené na rolích.
- Ověřte, zda použitá skupina není distribuční seznam. Intune na portálu Azure podporuje jenom uživatelské účty, které patří do skupin zabezpečení Služby Azure Active Directory. Zkontrolujte své skupiny v > **skupinách Azure**Portal nebo v Azure Portal > Azure Active  >  **Groups** **Directory**.

**Uživatel má příliš mnoho oprávnění pro přiřazenou roli Intune**

Poradit uživateli, **Intune**aby šel do rolí  >  **Intune Intune**  >  **Moje oprávnění**  >  **Exportovat** ke kontrole udělených oprávnění.

**Do role byla přidána skupina oboru, ale uživatelům v této roli se stále zobrazují ostatní uživatelé nebo zařízení**

Skupiny oborů neodfiltrují uživatele ani zařízení. Skupiny oborů:

- Omezte, komu mohou uživatelé přiřazovat zásady nebo aplikace.
- Povolit pouze určitým uživatelům spouštět vzdálené úlohy na zařízeních.

Další informace o skupinách oborů najdete v [tématu Řízení přístupu na základě rolí (RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Přidal(a) jsem uživatele do role Intune, ale pořád má plný přístup ke konzole pro správu Intune.**

Přejděte na Intune > **Users** na webu Azure Portal a ověřte, že uživatel není přiřazený k žádné z následujících rolí na webu Azure Portal:

- Globální správce
- Správce služby Intune
- Správce SharePointu

Další informace najdete v [tématu Řízení přístupu na základě rolí (RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problémy s přístupem**

Další informace najdete [v tématu Nemůžete se přihlásit k Office 365, Azure nebo Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).