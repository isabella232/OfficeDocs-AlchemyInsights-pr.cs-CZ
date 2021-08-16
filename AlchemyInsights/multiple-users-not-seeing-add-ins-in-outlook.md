---
title: Více uživatelů, kteří v aplikaci Outlook
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
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011797"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Více uživatelů, kteří v aplikaci Outlook

Pokud otestujte Outlook a žádný se zobrazí, použijte jako první krok řešení potíží rutinu **PowerShellu Get-OrganizationConfig** k dotazování na parametr _AppsForOfficeEnabled._ Pokud dotaz vrátí hodnotu **Nepravda**, nastavte tento parametr na **True** pomocí rutiny **Set-OrganizationConfig,** takže se doplňky zobrazí očekávaným způsobem.

Nedoporučujeme, aby byl parametr _AppsForOfficeEnabled_ nastavený na **False**. Hodnota **Nepravda** přepíše všechna výše uvedená nastavení rolí Správce a Uživatel a zabrání aktivaci všech nových aplikací libovolným uživatelem v organizaci.

Další informace najdete v článku Určení správců a uživatelů, kteří [můžou](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)instalovat a spravovat doplňky pro Outlook .