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
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944124"
---
# <a name="problems-using-the-intune-admin-console"></a>Problémy s používáním konzoly pro správu Intune

**"Přístup odepřen" při navigaci na portálu pro správu Intune.**

- Pokud jste členem vlastní role Intune, ujistěte se, že je k vašemu účtu přiřazená licence Intune nebo Enterprise Mobility Suite (EMS).
- Pokud ke správě zařízení Správce konfigurace, ověřte, že nejste součástí kolekce uživatelů Intune pro Správce konfigurace MDM.
- Ověřte, že jste v okně Role Intune přiřadili příslušná oprávnění řízení správy (RBAC) na základě rolí.
- Ověřte, že použitá skupina není distribuční seznam. Intune na portálu Azure portal podporuje jenom uživatelské účty, které patří do Azure Active Directory skupin zabezpečení. Zkontrolujte své skupiny na webu Azure Portal > **Intune** Groups nebo na  >  webu Azure Portal > **Azure Active Directory**.

**Uživatel má příliš mnoho oprávnění pro přiřazenou roli Intune.**

Doporučíte uživateli, aby šel do **rolí Intune** Intune Moje oprávnění Exportovat a zkontrolovat  >    >    >   udělená oprávnění.

**Přidal(a) jsem skupinu oborů do role, ale uživatelé v této roli pořád vidí další uživatele nebo zařízení.**

Skupiny oborů nevyfiltruje uživatele ani zařízení. Skupiny oborů:

- Omezte uživatele, kterým mohou přiřazovat zásady nebo aplikace.
- Povolte spouštění vzdálených úkolů jenom konkrétním uživatelům na zařízeních.

Další informace o skupinách oborů najdete v tématu Řízení přístupu založené na rolích [(RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Přidal(a) jsem uživatele do role Intune, ale pořád mají úplný přístup ke konzole pro správu Intune.**

Přejděte na Intune > **uživatelé** na portálu Azure Portal a ověřte, že uživatel není přiřazen k žádné z následujících rolí na portálu Azure Portal:

- Globální správce
- Správce služby Intune
- Správce SharePointu

Další informace najdete v tématu Řízení přístupu založené [na rolích (RBAC) s Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problémy s přístupem**

Další informace najdete v tématu Nemůžete se přihlásit k [Office 365, Azure](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)nebo Intune .