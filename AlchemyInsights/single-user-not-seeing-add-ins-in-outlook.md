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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="ff3f9-102">Jeden uživatel nemá v Outlooku žádné doplňky</span><span class="sxs-lookup"><span data-stu-id="ff3f9-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="ff3f9-103">Uživatel může být součástí role, která nemá správný parametr AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="ff3f9-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="ff3f9-104">Spuštěním této rutiny zjistíte, jestli je k uživateli přidružená správná role:</span><span class="sxs-lookup"><span data-stu-id="ff3f9-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="ff3f9-105">Get-ManagementRoleAssignment-RoleAssignee user@domain.com-delegování $false | Format-Table – Automatická role, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="ff3f9-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="ff3f9-106">Další informace najdete v tématu [Určení správců a uživatelů, kteří můžou nainstalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="ff3f9-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
