---
title: Blokování nahrávání schůzek uživateli
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035055"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="41016-102">Blokování nahrávání schůzek uživateli</span><span class="sxs-lookup"><span data-stu-id="41016-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="41016-103">Pokud potřebujete konkrétním uživatelům zabránit **v** zaznamenávání schůzek v Teams nebo je zablokovat, můžete to udělat pomocí nastavení zásad schůzek v Teams.</span><span class="sxs-lookup"><span data-stu-id="41016-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="41016-104">V Centru pro správu Microsoft Teams vypněte nastavení Povolit **cloudové** nahrávání v zásadách schůzky přiřazené tomuto uživateli.</span><span class="sxs-lookup"><span data-stu-id="41016-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="41016-105">Další informace najdete v tématu [Správa zásad schůzek v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="41016-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="41016-106">Pokud chcete ověřit, jestli má konkrétní uživatel povoleno nebo nemá zaznamenávat schůzky Teams, použijte diagnostiku podpory.</span><span class="sxs-lookup"><span data-stu-id="41016-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="41016-107">Spusťte nový dotaz podpory a zadejte **Diag: Meeting Recording** (Záznam schůzky): Diagnostika zkontroluje nastavení zásad pro zadaného uživatele a určí jejich nastavení zásad.</span><span class="sxs-lookup"><span data-stu-id="41016-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="41016-108">Nezapomeňte, že může trvat několik hodin, než se nová nastavení zásad projeví, takže pokud jste právě udělali změnu, počkejte několik hodin, než znovu spustit diagnostiku.</span><span class="sxs-lookup"><span data-stu-id="41016-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="41016-109">Další informace najdete v přehledu [Zapnutí nebo vypnutí nahrávání v cloudu](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="41016-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
