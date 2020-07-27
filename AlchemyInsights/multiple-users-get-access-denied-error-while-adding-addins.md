---
title: Více uživatelům se při přidávání doplňků v Outlooku zobrazí chyba odepření přístupu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423481"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Více uživatelům se při přidávání doplňků v Outlooku zobrazí chyba odepření přístupu

Můžete určit, kteří správci ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro aplikaci Outlook. Můžete také určit, kteří uživatelé ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro vlastní potřebu.

Podrobnosti naleznete [v tématu Určení správců a uživatelů, kteří mohou instalovat a spravovat doplňky pro aplikaci Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Chcete-li ověřit, zda jste uživateli úspěšně přiřadili oprávnění, <Role Name> nahraďte název role, kterou chcete ověřit, a spusťte následující příkaz v prostředí Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers

Tento příklad ukazuje, jak ověřit, komu jste přiřadili oprávnění k instalaci doplňků z Office Storu pro organizaci.

Powershell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Ve výsledcích Get-ManagementRoleAssignment zkontrolujte položky ve sloupci Efektivní uživatelé.

Podrobné informace o syntaxi a parametrech naleznete v [tématu Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 