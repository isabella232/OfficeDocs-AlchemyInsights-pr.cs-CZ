---
title: Microsoft Teams – přístup hostů
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: da9ecca062bd5f1dcc169657483ba53eb201def0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798369"
---
# <a name="microsoft-teams---guest-access"></a><span data-ttu-id="b2a99-102">Microsoft Teams – přístup hostů</span><span class="sxs-lookup"><span data-stu-id="b2a99-102">Microsoft Teams - Guest Access</span></span>

<span data-ttu-id="b2a99-103">Pokud potřebujete pomoct komunikovat s uživateli mimo vaši organizaci v aplikaci teams, musíte se rozhodnout, jestli chcete použít [přístup hostů nebo externí přístup (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), nebo můžete použít obojí.</span><span class="sxs-lookup"><span data-stu-id="b2a99-103">If you need help communicating with users outside your Organization in Teams, you need to decide whether to use [Guest Access or External Access (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), or you can use both.</span></span>

<span data-ttu-id="b2a99-104">Podívejte se, jaké jsou [rozdíly mezi](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) funkcemi dostupnými pro jednotlivé.</span><span class="sxs-lookup"><span data-stu-id="b2a99-104">Be sure to [review the differences](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) to understand the features available for each.</span></span>  <span data-ttu-id="b2a99-105">Například externí přístup (Federation) umožňuje komunikaci 1:1, jako je chat a přítomnost.</span><span class="sxs-lookup"><span data-stu-id="b2a99-105">For example, External access (federation) allows for 1:1 communications, like Chat and Presence.</span></span>  <span data-ttu-id="b2a99-106">Federované uživatele se ale nemohou zúčastnit spolupráce v týmu.</span><span class="sxs-lookup"><span data-stu-id="b2a99-106">Federated users cannot participate in Teams collaboration however.</span></span>  <span data-ttu-id="b2a99-107">Pokud chcete, aby se externí uživatel mohl připojit ke konverzacím kanálu nebo sdílet soubory, musíte zapnout přístup hostů.</span><span class="sxs-lookup"><span data-stu-id="b2a99-107">If you’d like an external user to join and participate in Teams Channel Conversations or Share Files, you’ll need to turn on Guest Access.</span></span>

<span data-ttu-id="b2a99-108">**Možnost 1: zapnutí přístupu hostů** </span><span class="sxs-lookup"><span data-stu-id="b2a99-108">**Option 1: Turn on Guest Access** </span></span>  
<span data-ttu-id="b2a99-109">V centru pro správu týmů přejděte na [Nastavení organizace > přístup hostů](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) a zapněte možnost povolit přístup hostů do týmů.</span><span class="sxs-lookup"><span data-stu-id="b2a99-109">In the Teams Admin Center, Go to [Org Wide Settings > Guest Access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) and turn on “Allow Guest Access in Teams”.</span></span>  <span data-ttu-id="b2a99-110">U tenanta s ostatními výchozími nastaveními by to mělo být.</span><span class="sxs-lookup"><span data-stu-id="b2a99-110">For a tenant with all other default settings, this should be all you need to do.</span></span>  <span data-ttu-id="b2a99-111">Chcete-li přizpůsobit konfiguraci přístupu pro hosty, postupujte podle pokynů v části [Kontrolní seznam pro přístup hostů](https://docs.microsoft.com/microsoftteams/guest-access-checklist).</span><span class="sxs-lookup"><span data-stu-id="b2a99-111">To customize your Guest Access configuration,  make sure you follow all the steps in the [Guest Access Checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist).</span></span> <span data-ttu-id="b2a99-112">Po dokončení musíte [počkat až 24 hodin, než](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) se nastavení projeví.</span><span class="sxs-lookup"><span data-stu-id="b2a99-112">Once you're completely done, you'll need to [wait up to 24 hours](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) for the settings to take effect.</span></span>

<span data-ttu-id="b2a99-113">Pokud jste si jistí, že jste dokončili všechny kroky v kontrolním seznamu, a je to víc než 24 hodin, zkuste [do týmu přidat hosta](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).</span><span class="sxs-lookup"><span data-stu-id="b2a99-113">If you’re confident you’ve completed all the steps in the Checklist, and it's been more than 24 hours, go ahead and try to [add a Guest to your Team](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).</span></span>

<span data-ttu-id="b2a99-114">Další informace, včetně videí, najdete [v tématu přístup hostů v Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).</span><span class="sxs-lookup"><span data-stu-id="b2a99-114">For more information, including how-to videos, see [Guest access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).</span></span>

<span data-ttu-id="b2a99-115">**Možnost 2: zapnutí externího přístupu (federace)** Pokud chcete taky zapnout externí přístup (federace), přejděte v centru pro správu týmů na nastavení pro celou organizaci [> externí přístup](https://admin.teams.microsoft.com/company-wide-settings/external-communications) a zapněte možnost Uživatelé mohou komunikovat s uživateli Skypu pro firmy a týmy a pak postupujte podle všech kroků, které [uživatelům týmů umožní chatovat a komunikovat s uživateli v jiné organizaci](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).</span><span class="sxs-lookup"><span data-stu-id="b2a99-115">**Option 2: Turn On External Access (Federation)** If you’d also like to turn on External Access (Federation), in the Teams Admin center go to [Org-wide Settings > External Access](https://admin.teams.microsoft.com/company-wide-settings/external-communications) and turn on "Users can communicate with Skype for Business and Teams users", and then follow all the steps in [Let your Teams users chat and communicate with users in another organization](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).</span></span>


