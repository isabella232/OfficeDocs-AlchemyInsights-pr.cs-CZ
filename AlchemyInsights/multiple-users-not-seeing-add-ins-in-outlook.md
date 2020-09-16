---
title: Víc uživatelů, kteří v Outlooku nevidí Doplňky
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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729864"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="34fa6-102">Víc uživatelů, kteří v Outlooku nevidí Doplňky</span><span class="sxs-lookup"><span data-stu-id="34fa6-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="34fa6-103">Pokud otestujete outlookové doplňky a nebudete se zobrazovat, jako první krok odstraňování potíží, použijte rutinu **Get-OrganizationConfig** PowerShellu k dotazování parametru _AppsForOfficeEnabled_ .</span><span class="sxs-lookup"><span data-stu-id="34fa6-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="34fa6-104">Pokud dotaz vrátí hodnotu **false**, nastavte tento parametr na **hodnotu true** pomocí rutiny **set-OrganizationConfig** , takže se doplňky zobrazí podle očekávání.</span><span class="sxs-lookup"><span data-stu-id="34fa6-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="34fa6-105">Nedoporučujeme, aby byl parametr _AppsForOfficeEnabled_ nastavený na **hodnotu false (NEPRAVDA**).</span><span class="sxs-lookup"><span data-stu-id="34fa6-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="34fa6-106">Hodnota **false** Přepisuje všechna výše uvedená nastavení administrativních a uživatelských rolí a zabraňuje aktivaci všech nových aplikací jakýmkoli uživatelem v organizaci.</span><span class="sxs-lookup"><span data-stu-id="34fa6-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="34fa6-107">Další informace najdete v tématu [Určení správců a uživatelů, kteří můžou nainstalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="34fa6-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>