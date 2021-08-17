---
title: Jeden uživatel, který v aplikaci Outlook
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
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050651"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Jeden uživatel, který v aplikaci Outlook

Uživatel může být součástí role, která nemá správný parametr AppsForOfficeEnabled. Spuštěním této rutiny zjistíte, jestli je správná role přidružená k uživateli:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegování $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Další informace najdete v článku Určení správců a uživatelů, kteří [můžou](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)instalovat a spravovat doplňky pro Outlook .
