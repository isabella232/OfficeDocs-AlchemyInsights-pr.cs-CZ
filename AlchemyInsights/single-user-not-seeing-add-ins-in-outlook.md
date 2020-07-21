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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="b8b36-102">Jeden uživatel nevidí doplňky v Outlooku</span><span class="sxs-lookup"><span data-stu-id="b8b36-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="b8b36-103">Uživatel může být součástí role, která nemá správný parametr AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="b8b36-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="b8b36-104">Spusťte tuto rutinu a zjistěte, zda je k uživateli přidružena správná role:</span><span class="sxs-lookup"><span data-stu-id="b8b36-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="b8b36-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegování $false | Formát-Tabulka -Automatická role,Název_role,Typ přiřazení_role</span><span class="sxs-lookup"><span data-stu-id="b8b36-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="b8b36-106">Další informace najdete [v tématu Určení správců a uživatelů, kteří můžou instalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="b8b36-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
