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
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="af69a-102">Více uživatelům se při přidávání doplňků v Outlooku zobrazí chyba odepření přístupu</span><span class="sxs-lookup"><span data-stu-id="af69a-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="af69a-103">Můžete určit, kteří správci ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro aplikaci Outlook.</span><span class="sxs-lookup"><span data-stu-id="af69a-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="af69a-104">Můžete také určit, kteří uživatelé ve vaší organizaci mají oprávnění k instalaci a správě doplňků pro vlastní potřebu.</span><span class="sxs-lookup"><span data-stu-id="af69a-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="af69a-105">Podrobnosti naleznete [v tématu Určení správců a uživatelů, kteří mohou instalovat a spravovat doplňky pro aplikaci Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="af69a-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="af69a-106">Chcete-li ověřit, zda jste uživateli úspěšně přiřadili oprávnění, <Role Name> nahraďte název role, kterou chcete ověřit, a spusťte následující příkaz v prostředí Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="af69a-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="af69a-107">Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="af69a-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="af69a-108">Tento příklad ukazuje, jak ověřit, komu jste přiřadili oprávnění k instalaci doplňků z Office Storu pro organizaci.</span><span class="sxs-lookup"><span data-stu-id="af69a-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="af69a-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="af69a-109">PowerShell</span></span>

<span data-ttu-id="af69a-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="af69a-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="af69a-111">Ve výsledcích Get-ManagementRoleAssignment zkontrolujte položky ve sloupci Efektivní uživatelé.</span><span class="sxs-lookup"><span data-stu-id="af69a-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="af69a-112">Podrobné informace o syntaxi a parametrech naleznete v [tématu Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="af69a-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 