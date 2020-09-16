---
title: Začínáme s živými událostmi v Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677272"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="98525-102">Začínáme s živými událostmi v Teams</span><span class="sxs-lookup"><span data-stu-id="98525-102">Getting started with Teams live events</span></span>

<span data-ttu-id="98525-103">Živé události Microsoft Teams jsou rozšířením týmových schůzek. Umožní vám plánovat a vytvářet události, které se streamují velkému množství online posluchačů.</span><span class="sxs-lookup"><span data-stu-id="98525-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="98525-104">K vytvoření živé události budete potřebovat následující:</span><span class="sxs-lookup"><span data-stu-id="98525-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="98525-105">Nejdřív ověřte, že jsou živé události aplikace Teams [ve vaší zemi a oblasti](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability). Živé události se zatím v některých zemích nepodporují.</span><span class="sxs-lookup"><span data-stu-id="98525-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="98525-106">Pokud jste přiřadili licence a nastavili zásady, ale stále nemůžete vytvořit živou událost v teams, je pravděpodobné, že jste v zemi nebo oblasti, kde jsou živé události zatím nedostupné.</span><span class="sxs-lookup"><span data-stu-id="98525-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="98525-107">[Licence Office 365 Enterprise E1, E3 nebo E5 nebo licence Office 365 A3 nebo A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="98525-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="98525-108">**Poznámka:** Vzhledem k nedávnému zvýšení využití Teams může po přiřazení licence Teams uživatelům trvat až 24 hodin, než se plně zprovozní.</span><span class="sxs-lookup"><span data-stu-id="98525-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="98525-109">Do té doby jim nebude možné přiřadit zásady Teams a pravděpodobně nebudou mít přístup k některým funkcím Teams, jako jsou volání a audiokonference.</span><span class="sxs-lookup"><span data-stu-id="98525-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="98525-110">Oprávnění [vytvářet živé události v centru pro správu Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="98525-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="98525-111">Oprávnění [vytvářet živé události v Microsoft Streamu](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (pro události produkované prostřednictvím externí vysílací aplikace nebo zařízení).</span><span class="sxs-lookup"><span data-stu-id="98525-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="98525-112">Plné týmové členství v organizaci (nemůže to být host ani osoba z jiné organizace).</span><span class="sxs-lookup"><span data-stu-id="98525-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="98525-113">Aktivované plánování soukromých schůzek, sdílení obrazovky a sdílení IP videa v zásadách týmových schůzek.</span><span class="sxs-lookup"><span data-stu-id="98525-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="98525-114">[Osvědčené postupy](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) pro živé události v Teams.</span><span class="sxs-lookup"><span data-stu-id="98525-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="98525-115">Další informace najdete v článku [Začínáme s živými událostmi v Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="98525-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>