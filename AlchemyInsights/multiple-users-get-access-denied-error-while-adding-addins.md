---
title: Více uživatelům se při přidávání doplňků v Outlooku zobrazuje chyba odepření přístupu
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
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724356"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Více uživatelům se při přidávání doplňků v Outlooku zobrazuje chyba odepření přístupu

Můžete určit, kteří správci ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro Outlook. Můžete také určit, kteří uživatelé ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro jejich vlastní potřebu.

Podrobnosti najdete v tématu [Určení správců a uživatelů, kteří můžou nainstalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Pokud chcete ověřit, jestli jste úspěšně přiřadili oprávnění pro uživatele, nahraďte <Role Name> název role, kterou chcete ověřit, a v PowerShellu Exchange Online spusťte následující příkaz:

Get-ManagementRoleAssignment-role " <Role Name> "-GetEffectiveUsers

Tento příklad ukazuje, jak ověřit, komu jste přiřadili oprávnění k instalaci doplňků z Office Storu pro organizaci.

PowerShell

-Role "aplikace pro organizaci org" – GetEffectiveUsers

Ve výsledcích, Get-ManagementRoleAssignment, zkontrolujte položky ve sloupci efektivní uživatelé.

Podrobné informace o syntaxi a parametrech najdete v tématu [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 