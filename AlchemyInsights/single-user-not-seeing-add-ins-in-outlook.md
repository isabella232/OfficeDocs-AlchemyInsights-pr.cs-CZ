---
title: Jeden uživatel nemá v Outlooku žádné doplňky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719658"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Jeden uživatel nemá v Outlooku žádné doplňky

Uživatel může být součástí role, která nemá správný parametr AppsForOfficeEnabled. Spuštěním této rutiny zjistíte, jestli je k uživateli přidružená správná role:

Get-ManagementRoleAssignment-RoleAssignee user@domain.com-delegování $false | Format-Table – Automatická role, RoleAssigneeName, RoleAssigneeType

Další informace najdete v tématu [Určení správců a uživatelů, kteří můžou nainstalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
