---
title: Jeden uživatel nevidí doplňky v Outlooku
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197768"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Jeden uživatel nevidí doplňky v Outlooku

Uživatel může být součástí role, která nemá správný parametr AppsForOfficeEnabled. Spusťte tuto rutinu a zjistěte, zda je k uživateli přidružena správná role:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegování $false | Formát-Tabulka -Automatická role,Název_role,Typ přiřazení_role

Další informace najdete [v tématu Určení správců a uživatelů, kteří můžou instalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
