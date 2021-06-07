---
title: Povolení Teams webináře
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793582"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="83293-102">Povolení Teams webináře</span><span class="sxs-lookup"><span data-stu-id="83293-102">Enable Teams Webinars</span></span>

<span data-ttu-id="83293-103">Webináře jsou ve výchozím nastavení povolené.</span><span class="sxs-lookup"><span data-stu-id="83293-103">Webinars are enabled by default.</span></span> <span data-ttu-id="83293-104">Pomocí příkazů PowerShellu můžete spravovat, kdo Teams plánovat a registrovat Teams Teams webináře.</span><span class="sxs-lookup"><span data-stu-id="83293-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="83293-105">Všichni uživatelé, kteří mohou vytvořit schůzku, mohou také vytvořit webinářovou schůzku.</span><span class="sxs-lookup"><span data-stu-id="83293-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="83293-106">Pokud chcete spravovat, kdo může plánovat Teams webináře, použijte *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="83293-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="83293-107">Ve výchozím nastavení *je funkce WhoCanRegister* povolená a nastavená na **Everyone (Všichni).**</span><span class="sxs-lookup"><span data-stu-id="83293-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="83293-108">Pokud chcete registraci schůzky vypnout, nastavte *AllowMeetingRegistration na* **False**.</span><span class="sxs-lookup"><span data-stu-id="83293-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="83293-109">Pokud chcete tato nastavení změnit, musíte si [Teams PowerShellu](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="83293-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="83293-110">Zásady schůzek se také vynucuje na Teams webináře.</span><span class="sxs-lookup"><span data-stu-id="83293-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="83293-111">Pokud je například anonymní připojení vypnuté v nastavení schůzky, anonymní uživatelé se neschová k webináři.</span><span class="sxs-lookup"><span data-stu-id="83293-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="83293-112">Další informace o konfiguraci, kdo se může registrovat pro webináře, najdete v tématu Konfigurace, kdo se [může zaregistrovat pro webináře](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="83293-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="83293-113">Další informace o nastavení microsoftových seznamů najdete v tématu [Nastavení řízení pro seznamy Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="83293-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>