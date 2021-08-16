---
title: Více uživatelům se při přidávání doplňků do Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065385"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Více uživatelům se při přidávání doplňků do Outlook

Můžete určit, kteří správci ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro Outlook. Můžete taky určit, kteří uživatelé ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro vlastní použití.

Podrobnosti najdete v článku Určení správců a uživatelů, kteří [můžou](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)instalovat a spravovat doplňky pro Outlook .

Pokud chcete ověřit, že jste uživateli úspěšně přiřadili oprávnění, nahraďte ho názvem role, kterou chcete ověřit, a spusťte následující příkaz v <Role Name> Exchange Online PowerShellu:

Get-ManagementRoleAssignment -Role " <Role Name> " - GetEffectiveUsers

Tento příklad ukazuje, jak ověřit, komu jste přiřadili oprávnění k instalaci doplňků z Office Store pro organizaci.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Ve výsledcích Get-ManagementRoleAssignment zkontrolujte položky ve sloupci Efektivní uživatelé.

Podrobné informace o syntaxi a parametrech najdete v [tématu Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 