---
title: Skrytí nebo zobrazení týmů nebo skupin Office 365 v seznamu adres
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811449"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrytí nebo zobrazení týmů nebo skupin Office 365 v seznamu adres

Pomocí následujícího příkazu EXO PowerShell můžete skrýt nebo zobrazit týmy nebo skupiny Office 365 v seznamech adres (globálním adresáři) klientů Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Pomocí následujícího příkazu EXO PowerShell můžete skrýt nebo zobrazit týmy nebo skupiny Office 365 v klientech Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Podrobné pokyny najdete v tématu [Skrytí skupin Office 365 v globálním adresáři a klientech Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
