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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088389"
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
