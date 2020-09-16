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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Víc uživatelů, kteří v Outlooku nevidí Doplňky

Pokud otestujete outlookové doplňky a nebudete se zobrazovat, jako první krok odstraňování potíží, použijte rutinu **Get-OrganizationConfig** PowerShellu k dotazování parametru _AppsForOfficeEnabled_ . Pokud dotaz vrátí hodnotu **false**, nastavte tento parametr na **hodnotu true** pomocí rutiny **set-OrganizationConfig** , takže se doplňky zobrazí podle očekávání.

Nedoporučujeme, aby byl parametr _AppsForOfficeEnabled_ nastavený na **hodnotu false (NEPRAVDA**). Hodnota **false** Přepisuje všechna výše uvedená nastavení administrativních a uživatelských rolí a zabraňuje aktivaci všech nových aplikací jakýmkoli uživatelem v organizaci.

Další informace najdete v tématu [Určení správců a uživatelů, kteří můžou nainstalovat a spravovat doplňky pro Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).