---
title: Nastavení zásad schůzky
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825436"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="3de10-102">Správa zásad schůzek v Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3de10-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="3de10-103">**Poznámka: Může trvat až 24 hodin, než se změny zásad projeví pro uživatele.**</span><span class="sxs-lookup"><span data-stu-id="3de10-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="3de10-104">V nově vytvořených zásadách možná nebudete moct okamžitě dělat změny. počkejte 4 hodiny a zkuste znovu upravit nově vytvořenou zásadu.</span><span class="sxs-lookup"><span data-stu-id="3de10-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="3de10-105">Zásady schůzek slouží k řízení funkcí, které jsou dostupné účastníkům schůzky pro schůzky naplánované uživateli ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="3de10-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="3de10-106">Některé funkce zásad schůzek ještě nemusí být implementované v Centru pro správu Teams (ty jsou v dokumentaci označené jako "brzy").</span><span class="sxs-lookup"><span data-stu-id="3de10-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="3de10-107">V tomto případě nebo pokud se vám v Centru pro správu Microsoft Teams zobrazí chybová zpráva, třeba "Zásady teď nemůžeme aktualizovat, ale zkuste to znovu později", doporučujeme k vytvoření nebo úpravě zásad schůzek v Teams použít PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3de10-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="3de10-108">Další informace o zásadách schůzek najdete v těchto zdrojích:</span><span class="sxs-lookup"><span data-stu-id="3de10-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="3de10-109">Další informace o vytváření zásad, provádění změn a přiřazování uživatelů k zásadám najdete v tématu Správa zásad [schůzek v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="3de10-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="3de10-110">Pokud chcete provádět změny zásad pomocí rutin PowerShellu, podívejte se na [přehled Teams PowerShellu.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="3de10-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="3de10-111">Pro zásady schůzek v Teams musíte použít modul [PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Skypu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="3de10-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="3de10-112">Další informace najdete v dokumentaci rutin [\*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="3de10-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

