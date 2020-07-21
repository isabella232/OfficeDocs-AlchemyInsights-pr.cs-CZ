---
title: Více uživatelům, kteří v Outlooku nevidí doplňky
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197772"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="66f15-102">Více uživatelům, kteří v Outlooku nevidí doplňky</span><span class="sxs-lookup"><span data-stu-id="66f15-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="66f15-103">Pokud otestujete doplňky aplikace Outlook a žádné se nezobrazí jako první krok řešení potíží, použijte rutinu **Get-OrganizationConfig** PowerShell k dotazování na parametr _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="66f15-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="66f15-104">Pokud dotaz vrátí hodnotu **False**, nastavte tento parametr na **Hodnotu True** pomocí rutiny **Set-OrganizationConfig,** takže doplňky se zobrazí podle očekávání.</span><span class="sxs-lookup"><span data-stu-id="66f15-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="66f15-105">Nedoporučujeme, aby _appsforofficeenabled_ parametr je nastavena na **False**.</span><span class="sxs-lookup"><span data-stu-id="66f15-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="66f15-106">Hodnota **False** přepíše všechna výše uvedená nastavení rolí Správce a Uživatel a zabrání aktivaci nových aplikací libovolným uživatelem v organizaci.</span><span class="sxs-lookup"><span data-stu-id="66f15-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="66f15-107">Další informace naleznete [v tématu Určení správců a uživatelů, kteří mohou instalovat a spravovat doplňky pro aplikaci Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="66f15-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>