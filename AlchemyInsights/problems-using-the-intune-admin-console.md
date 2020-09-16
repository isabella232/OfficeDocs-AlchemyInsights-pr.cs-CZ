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
# <a name="problems-using-the-intune-admin-console"></a>Problémy s používáním konzoly pro správu Intune

**Při navigaci na portálu pro správu Intune se zobrazí zpráva Access denied (přístup odepřen).**

- Pokud jste členem vlastní role Intune, ujistěte se, že k vašemu účtu je přiřazená licence EMS (Intune nebo Enterprise mobility).
- Pokud ke správě zařízení používáte nástroj Configuration Manager, ověřte, že nejste součástí Intune User Collection pro MDM Configuration Manager.
- Zkontrolujte, jestli máte v okně role Intune přiřazená oprávnění řízení správy založené na rolích (RBAC).
- Ověřte, že použitá skupina není distribuční seznam. Intune na Azure Portal podporuje jenom uživatelské účty patřící do skupin zabezpečení Azure Active Directory. Prohlédněte si skupiny v Azure Portalu > skupiny **Intune**  >  **Groups**nebo v Azure Portal > **Azure Active Directory**.

**Uživatel má příliš mnoho oprávnění k přiřazené roli Intune.**

Informujte uživatele, aby přešel na **Intune**  >  **Intune roles**Intune  >  **My permissions**  >  **Export**

**Do role přidal (a) skupinu oborů, ale uživatelé v dané roli pořád uvidí další uživatele nebo zařízení.**

Skupiny oborů nefiltrují uživatele nebo zařízení. Skupiny oborů:

- Omezte počet uživatelů, kteří můžou přiřazovat zásady nebo aplikace.
- Povolte spouštění vzdálených úloh na zařízeních pouze konkrétním uživatelům.

Další informace o skupinách oborů najdete v tématu  [řízení přístupu založeném na rolích (RBAC) v Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Do role Intune jsem přidal (a), ale pořád má úplný přístup ke konzole správce Intune.**

Přejděte na Intune > **uživatele** na portálu Azure a ověřte, jestli uživatel nemá přiřazenou žádnou z následujících rolí na portálu Azure:

- Globální správce
- Intune – Správce služby
- Správce SharePointu

Další informace najdete v tématu [řízení přístupu založeném na rolích (RBAC) v Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problémy s přístupem**

Další informace najdete v článku [nemůžete se přihlásit k Office 365, Azure nebo Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).