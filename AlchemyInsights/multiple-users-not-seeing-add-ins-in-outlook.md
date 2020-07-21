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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Více uživatelům, kteří v Outlooku nevidí doplňky

Pokud otestujete doplňky aplikace Outlook a žádné se nezobrazí jako první krok řešení potíží, použijte rutinu **Get-OrganizationConfig** PowerShell k dotazování na parametr _AppsForOfficeEnabled._ Pokud dotaz vrátí hodnotu **False**, nastavte tento parametr na **Hodnotu True** pomocí rutiny **Set-OrganizationConfig,** takže doplňky se zobrazí podle očekávání.

Nedoporučujeme, aby _appsforofficeenabled_ parametr je nastavena na **False**. Hodnota **False** přepíše všechna výše uvedená nastavení rolí Správce a Uživatel a zabrání aktivaci nových aplikací libovolným uživatelem v organizaci.

Další informace naleznete [v tématu Určení správců a uživatelů, kteří mohou instalovat a spravovat doplňky pro aplikaci Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).