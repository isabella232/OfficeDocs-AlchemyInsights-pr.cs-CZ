---
title: Používání Giphů v konverzacích Teams
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982436"
---
# <a name="using-giphys-in-teams-conversations"></a>Používání Giphů v konverzacích Teams

Giphů Access ve službě Teams chat je ve výchozím nastavení povolený. Jako správce můžete určit, jestli jsou Giphů k dispozici uživatelům [nastavením zásad pro zasílání zpráv](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) a zajistit, aby se **v konverzacích používaly giphů** . **On**

Pokud soubory GIF nefungují podle očekávání v konverzacích teams, ověřte:

[Zásady zasílání zpráv](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) musí umožňovat giphů. Ověření pomocí rutin PowerShellu:

- Ověřte, že můžete [spravovat týmy pomocí PowerShellu](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Spusťte příkaz PowerShell [Get-CsTeamsMessagingPolicy-identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) a ověřte, že je **AllowGiphy** nastaven na **hodnotu true**.
- Pokud je **AllowGiphy** nastaven na **false (NEPRAVDA** ), spusťte následující PowerShell Command [set-CsTeamsMessagingPolicy-identity Global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Chcete-li povolit přístup k adrese URL Giphy, je třeba povolit [volitelné připojení](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Pokud máte pro tenanta nastavené několik zásad zasílání zpráv v teams, můžete určit identitu zásady přiřazené ovlivněnému uživateli pomocí příkazu PowerShell [Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vyberte TeamsMessagingPolicy.
