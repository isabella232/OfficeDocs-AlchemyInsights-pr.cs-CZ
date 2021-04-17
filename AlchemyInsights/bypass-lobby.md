---
title: Obejít předsálí
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820027"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="28155-102">Řízení nastavení předsálí a úrovně účasti v Teams</span><span class="sxs-lookup"><span data-stu-id="28155-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="28155-103">Pokud chcete všem, včetně vytáčených, externích a anonymních uživatelů povolit obejít předsálí, použijte k provedení tohoto úkolu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="28155-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="28155-104">Tady je příklad úpravy zásad globální schůzky pro vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="28155-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="28155-105">Tato rutina momentálně vyžaduje použití modulu PowerShell Skypu pro firmy.</span><span class="sxs-lookup"><span data-stu-id="28155-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="28155-106">Pokud chcete tuto rutinu nastavit, podívejte se na správu [zásad přes PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="28155-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="28155-107">Jakmile nastavíte zásadu, musíte ji použít pro uživatele. nebo pokud jste změnili globální zásadu, automaticky se použije pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="28155-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="28155-108">Pokud chcete změnit zásady, musíte počkat minimálně 4 hodiny **až 24** hodin, než se zásady projeví.</span><span class="sxs-lookup"><span data-stu-id="28155-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="28155-109">Před provedením těchto změn si před provedením těchto změn prohlédněte dokumentaci, abyste přesně pochopili, co to umožňuje.</span><span class="sxs-lookup"><span data-stu-id="28155-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="28155-110">Principy řízení zásad v předsálí schůzek v Teams</span><span class="sxs-lookup"><span data-stu-id="28155-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="28155-111">Tato nastavení řídí, kteří účastníci schůzky čekají v předsálí před přijetím ke schůzce, a úroveň účasti, kterou mají účastníci schůzky povolenou na schůzce.</span><span class="sxs-lookup"><span data-stu-id="28155-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="28155-112">PowerShell můžete použít k aktualizaci nastavení zásad schůzky, která ještě nebyla implementovaná (označená jako "brzy") v Centru pro správu Teams.</span><span class="sxs-lookup"><span data-stu-id="28155-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="28155-113">Níže najdete příklad rutiny PowerShellu, která umožňuje všem uživatelům obejít předsálí.</span><span class="sxs-lookup"><span data-stu-id="28155-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="28155-114">[Automatické přijetí lidí](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) je zásada pro organizátory, která určuje, jestli se lidé připojují ke schůzce přímo, nebo čekat v předsálí, dokud je nepřijme ověřený uživatel.</span><span class="sxs-lookup"><span data-stu-id="28155-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="28155-115">Povolit [anonymním](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) lidem zahájit schůzku je zásada pro organizátory, která určuje, jestli se anonymní lidé, včetně uživatelů B2B a federovaných uživatelů, mohou připojit ke schůzce uživatele bez účasti ověřeného uživatele z organizace.</span><span class="sxs-lookup"><span data-stu-id="28155-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="28155-116">Povolit [uživatelům](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) vytáčení obejít předsálí **(už** brzy) je zásada pro organizátory, která určuje, jestli se lidé, kteří se telefonicky připojují ke schůzce přímo, nebo čekají v předsálí bez ohledu na nastavení Automaticky připustit **lidi.**</span><span class="sxs-lookup"><span data-stu-id="28155-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="28155-117">Povolit organizátorům přepsat nastavení předsálí [(už](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **brzy)** je zásada pro organizátory, která určuje, jestli  organizátor schůzky může přepsat nastavení předsálí nastavené správcem v části Automaticky připustit lidi a Povolit uživatelům vytáčení obcházet předsálí při plánování nové schůzky. </span><span class="sxs-lookup"><span data-stu-id="28155-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="28155-118">**Poznámka:** Úplný [přehled zásad schůzek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) v Microsoft Teams najdete v článku Správa zásad schůzek v Teams.</span><span class="sxs-lookup"><span data-stu-id="28155-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
