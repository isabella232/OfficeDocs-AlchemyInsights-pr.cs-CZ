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
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="3fba6-102">Více uživatelům se při přidávání doplňků v Outlooku zobrazuje chyba odepření přístupu</span><span class="sxs-lookup"><span data-stu-id="3fba6-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="3fba6-103">Můžete určit, kteří správci ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro Outlook.</span><span class="sxs-lookup"><span data-stu-id="3fba6-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="3fba6-104">Můžete také určit, kteří uživatelé ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro jejich vlastní potřebu.</span><span class="sxs-lookup"><span data-stu-id="3fba6-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="3fba6-105">Podrobnosti najdete v tématu [Určení správců a uživatelů, kteří můžou nainstalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="3fba6-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="3fba6-106">Pokud chcete ověřit, jestli jste úspěšně přiřadili oprávnění pro uživatele, nahraďte <Role Name> název role, kterou chcete ověřit, a v PowerShellu Exchange Online spusťte následující příkaz:</span><span class="sxs-lookup"><span data-stu-id="3fba6-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="3fba6-107">Get-ManagementRoleAssignment-role " <Role Name> "-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="3fba6-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="3fba6-108">Tento příklad ukazuje, jak ověřit, komu jste přiřadili oprávnění k instalaci doplňků z Office Storu pro organizaci.</span><span class="sxs-lookup"><span data-stu-id="3fba6-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="3fba6-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="3fba6-109">PowerShell</span></span>

<span data-ttu-id="3fba6-110">-Role "aplikace pro organizaci org" – GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="3fba6-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="3fba6-111">Ve výsledcích, Get-ManagementRoleAssignment, zkontrolujte položky ve sloupci efektivní uživatelé.</span><span class="sxs-lookup"><span data-stu-id="3fba6-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="3fba6-112">Podrobné informace o syntaxi a parametrech najdete v tématu [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="3fba6-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 