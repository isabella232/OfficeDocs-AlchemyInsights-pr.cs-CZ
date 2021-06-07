---
title: Správa registrace webináře
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793618"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="c02b0-102">Správa registrace webináře</span><span class="sxs-lookup"><span data-stu-id="c02b0-102">Manage webinar registration</span></span>

<span data-ttu-id="c02b0-103">Pomocí příkazů Powershellu můžete Teams, kdo se Teams webináře zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="c02b0-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="c02b0-104">Informace o Teams PowerShellu najdete [v Teams PowerShellu.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="c02b0-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="c02b0-105">Ve výchozím nastavení *je funkce WhoCanRegister* povolená a nastavená na **Hodnotu EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="c02b0-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="c02b0-106">Pokud chcete povolit registraci všem uživatelům, včetně anonymních  uživatelů, musíte pomocí příkazu Powershellu nastavit zásady schůzky na Všichni:</span><span class="sxs-lookup"><span data-stu-id="c02b0-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="c02b0-107">**Poznámka:** Pokud je anonymní připojení v nastavení schůzky vypnuté, anonymní uživatelé se neschová k webináři.</span><span class="sxs-lookup"><span data-stu-id="c02b0-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="c02b0-108">Další informace a povolení tohoto nastavení najdete v tématu [Správa nastavení schůzky v Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="c02b0-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="c02b0-109">Pokud chcete registraci schůzky vypnout, nastavte *AllowMeetingRegistration na* **False**.</span><span class="sxs-lookup"><span data-stu-id="c02b0-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="c02b0-110">Další informace o konfiguraci, kdo se může registrovat pro webináře, najdete v tématu Konfigurace, kdo se [může zaregistrovat pro webináře](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="c02b0-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="c02b0-111">Další informace o nastavení microsoftových seznamů najdete v tématu [Nastavení řízení pro seznamy Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="c02b0-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
