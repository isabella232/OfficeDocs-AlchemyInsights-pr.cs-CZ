---
title: Vynechat předsálí
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684943"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="afb11-102">Řízení nastavení a úrovně účasti v Teams</span><span class="sxs-lookup"><span data-stu-id="afb11-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="afb11-103">Pokud chcete umožnit všem, včetně vytáčeného připojení, externích a anonymních uživatelů, **vycházet z**této věci pomocí PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="afb11-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="afb11-104">Tady je příklad změny globální zásady pro schůzku ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="afb11-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="afb11-105">Tato rutina momentálně vyžaduje použití modulu PowerShell pro firmy.</span><span class="sxs-lookup"><span data-stu-id="afb11-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="afb11-106">Pokud chcete tuto rutinu nastavit, přečtěte si [zásady správy prostřednictvím PowerShellu](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="afb11-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="afb11-107">Po nastavení zásad je potřeba ji použít pro uživatele. nebo pokud jste změnili globální zásadu, automaticky se použije pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="afb11-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="afb11-108">Pro každou změnu zásad musíte počkat alespoň **4 hodiny až 24 hodin** , aby zásady vstoupily v platnost.</span><span class="sxs-lookup"><span data-stu-id="afb11-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="afb11-109">Před provedením těchto změn si přečtěte níže uvedenou dokumentaci, abyste pochopili přesně to, co umožňuje.</span><span class="sxs-lookup"><span data-stu-id="afb11-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="afb11-110">Principy řízení zásad v případě týmů</span><span class="sxs-lookup"><span data-stu-id="afb11-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="afb11-111">Tato nastavení určují, které účastníky schůzky před přijetím do schůzky čekají v předsálí, a úroveň jejich účasti, která je na schůzce povolená.</span><span class="sxs-lookup"><span data-stu-id="afb11-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="afb11-112">Pomocí PowerShellu můžete aktualizovat nastavení zásad schůzky, která nejsou v centru pro správu Teams dosud implementovaná (označená příznakem brzy).</span><span class="sxs-lookup"><span data-stu-id="afb11-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="afb11-113">V následujícím článku najdete příklad rutiny PowerShellu, která umožňuje všem uživatelům vynechat předsálí.</span><span class="sxs-lookup"><span data-stu-id="afb11-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="afb11-114">[Automaticky připustit uživatele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) : Jedná se o zásadu, která určuje, jestli se lidé ke schůzce můžou připojit přímo nebo počkat, dokud je nepřijmou ověřený uživatel.</span><span class="sxs-lookup"><span data-stu-id="afb11-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="afb11-115">[Povolit zahájení schůzky anonymním uživatelům](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je zásada, která určuje, jestli se může anonymním lidem, včetně B2B a federovaných uživatelů, připojit ke schůzce uživatele bez ověřeného uživatele z organizace v docházkě.</span><span class="sxs-lookup"><span data-stu-id="afb11-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="afb11-116">[Povolit uživatelům vytáčené komunikace obejít předsálí](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**již brzy**) je zásada pro jednotlivé organizátory, která určuje, jestli se uživatelé, kteří používají telefon, můžou připojit ke schůzce přímo nebo počkat v předsálí bez ohledu na nastavení **automaticky povolit uživatele** .</span><span class="sxs-lookup"><span data-stu-id="afb11-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="afb11-117">[Povolit organizátorům přepsat nastavení](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) informací (**už brzy**) je zásada pro jednotlivé organizátory, která určuje, jestli může organizátor schůzky přepsat nastavení s informacemi, které správce nastavil **automaticky** a **povolí uživatelům vytáčeného připojení, aby** při plánování nové schůzky tento předsálí vycházel.</span><span class="sxs-lookup"><span data-stu-id="afb11-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="afb11-118">**Poznámka:** Přečtěte si téma [Správa zásad schůzky v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , kde najdete kompletní přehled zásad schůzky v Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="afb11-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
