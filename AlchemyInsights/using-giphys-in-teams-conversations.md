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
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="82f34-102">Používání Giphů v konverzacích Teams</span><span class="sxs-lookup"><span data-stu-id="82f34-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="82f34-103">Giphů Access ve službě Teams chat je ve výchozím nastavení povolený.</span><span class="sxs-lookup"><span data-stu-id="82f34-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="82f34-104">Jako správce můžete určit, jestli jsou Giphů k dispozici uživatelům [nastavením zásad pro zasílání zpráv](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) a zajistit, aby se **v konverzacích používaly giphů** . **On**</span><span class="sxs-lookup"><span data-stu-id="82f34-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="82f34-105">Pokud soubory GIF nefungují podle očekávání v konverzacích teams, ověřte:</span><span class="sxs-lookup"><span data-stu-id="82f34-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="82f34-106">[Zásady zasílání zpráv](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) musí umožňovat giphů.</span><span class="sxs-lookup"><span data-stu-id="82f34-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="82f34-107">Ověření pomocí rutin PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="82f34-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="82f34-108">Ověřte, že můžete [spravovat týmy pomocí PowerShellu](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="82f34-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="82f34-109">Spusťte příkaz PowerShell [Get-CsTeamsMessagingPolicy-identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) a ověřte, že je **AllowGiphy** nastaven na **hodnotu true**.</span><span class="sxs-lookup"><span data-stu-id="82f34-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="82f34-110">Pokud je **AllowGiphy** nastaven na **false (NEPRAVDA** ), spusťte následující PowerShell Command [set-CsTeamsMessagingPolicy-identity Global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="82f34-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="82f34-111">Chcete-li povolit přístup k adrese URL Giphy, je třeba povolit [volitelné připojení](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="82f34-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="82f34-112">Pokud máte pro tenanta nastavené několik zásad zasílání zpráv v teams, můžete určit identitu zásady přiřazené ovlivněnému uživateli pomocí příkazu PowerShell [Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vyberte TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="82f34-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
