---
title: Nastavení zásad schůzky
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794327"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="5d6f9-102">Správa zásad schůzky v Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5d6f9-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="5d6f9-103">**Poznámka: změny zásad se projeví až až za 24 hodin.**</span><span class="sxs-lookup"><span data-stu-id="5d6f9-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="5d6f9-104">Je možné, že nebudete moct okamžitě měnit nově vytvořené zásady. Počkejte 4 hodiny a zkuste znovu změnit nově vytvořenou zásadu.</span><span class="sxs-lookup"><span data-stu-id="5d6f9-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="5d6f9-105">Zásady schůzky se používají k řízení funkcí, které jsou k dispozici účastníkům schůzky, které jsou naplánované uživateli ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="5d6f9-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="5d6f9-106">Některé funkce zásad schůzky se zatím neaktivují v centru pro správu týmů (v dokumentaci jsou označené jako nadcházející).</span><span class="sxs-lookup"><span data-stu-id="5d6f9-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="5d6f9-107">V tomto případě nebo pokud se vám zobrazí chybová zpráva "Nemůžeme tuto zásadu aktualizovat, ale zkuste to později" v centru pro správu Microsoft Teams doporučujeme použít PowerShell k vytvoření nebo úpravě zásad schůzky v Teams.</span><span class="sxs-lookup"><span data-stu-id="5d6f9-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="5d6f9-108">Další informace o zásadách schůzky najdete v následujících zdrojích:</span><span class="sxs-lookup"><span data-stu-id="5d6f9-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="5d6f9-109">Informace o vytváření zásad, provádění změn a přiřazování uživatelů k zásadám najdete v tématu [Správa zásad schůzky v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="5d6f9-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="5d6f9-110">Informace o změnách zásad pomocí rutin PowerShellu najdete v tématu [Team PowerShell – přehled](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="5d6f9-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="5d6f9-111">Potřebujete použít [modul PowerShell Skypu pro firmy](https://www.microsoft.com/download/details.aspx?id=39366) pro zásady schůzky v Teams.</span><span class="sxs-lookup"><span data-stu-id="5d6f9-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="5d6f9-112">Další informace najdete v [dokumentaci rutin \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="5d6f9-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

