---
title: Používání Giphys v Teams konverzacích
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323513"
---
# <a name="using-giphys-in-teams-conversations"></a>Používání Giphys v Teams konverzacích

Giphys access in Teams chat is enabled by default. Jako správce můžete nastavit, jestli jsou uživatelé giphys k dispozici, [nastavením](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) zásad zasílání zpráv a zajištěním toho, aby funkce **Používat Giphys** v konverzacích byla **na .**

Pokud gify v konverzacích nefungují Teams očekávaným způsobem, ověřte:

Zásady [zasílání zpráv](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) musí povolit Giphys. Ověření pomocí rutin PowerShellu:

- Ověřte, že můžete [spravovat Teams pomocí PowerShellu](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Spusťte příkaz [PowerShellu Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) a ověřte, jestli **je allowgiphy** nastavená na **TRUE**.
- Pokud **je možnost AllowGiphy** nastavená na **FALSE**, spusťte následující příkaz PowerShellu [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Aby bylo možné](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) povolit přístup k adrese URL Giphy, je potřeba povolit volitelné připojené prostředí.

**Poznámka:** Pokud máte pro tenanta nakonfigurovaných více zásad zasílání zpráv Teams, můžete určit identitu zásad přiřazenou ovlivněným uživatelům pomocí příkazu [PowerShellu Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vyberte TeamsMessagingPolicy.
