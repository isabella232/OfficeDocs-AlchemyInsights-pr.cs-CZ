---
title: Skrytí nebo skrytí skupin nebo týmů Office 365 ze seznamu adres
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225344"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrytí nebo skrytí skupin nebo týmů Office 365 ze seznamu adres

Pomocí následujícího příkazu EXO PowerShell můžete skrýt nebo skrýt skupiny/týmy Office 365 ze seznamů adres (GAL) klientů Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Pomocí následujícího příkazu EXO PowerShell můžete skrýt nebo skrýt skupinu/týmy Office365 před klienty Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Podrobné pokyny naleznete v [tématu Skrytí skupin Office 365 z globálního seznamu adres a klientů Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
