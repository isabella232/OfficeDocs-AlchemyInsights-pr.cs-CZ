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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="d72ec-102">Skrytí nebo skrytí skupin nebo týmů Office 365 ze seznamu adres</span><span class="sxs-lookup"><span data-stu-id="d72ec-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="d72ec-103">Pomocí následujícího příkazu EXO PowerShell můžete skrýt nebo skrýt skupiny/týmy Office 365 ze seznamů adres (GAL) klientů Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="d72ec-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="d72ec-104">Pomocí následujícího příkazu EXO PowerShell můžete skrýt nebo skrýt skupinu/týmy Office365 před klienty Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="d72ec-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="d72ec-105">Podrobné pokyny naleznete v [tématu Skrytí skupin Office 365 z globálního seznamu adres a klientů Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="d72ec-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
