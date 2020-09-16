---
title: Návrat k dřívějšímu buildu Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1741"
- "9000140"
ms.openlocfilehash: 9f6a812def2b46bf32d836781d0336aea5ba3ed1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727812"
---
# <a name="roll-back-to-an-earlier-build-of-office"></a><span data-ttu-id="129e6-102">Návrat k dřívějšímu buildu Office</span><span class="sxs-lookup"><span data-stu-id="129e6-102">Roll back to an earlier build of Office</span></span>

<span data-ttu-id="129e6-103">Pokud se chcete vrátit k dřívější verzi buildu nebo verze Microsoft 365, přečtěte si [článek Jak se vrátit k dřívější verzi Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span><span class="sxs-lookup"><span data-stu-id="129e6-103">To revert to an earlier Microsoft 365 Apps build or version, see [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span></span> <span data-ttu-id="129e6-104">Pokud chcete přejít z jednoho předplatného Microsoft 365 na jiný, přečtěte si článek  [Přechod na jiný plán microsoft 365 pro firmy](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="129e6-104">To switch from one Microsoft 365 subscription to another, see  [Switch to a different Microsoft 365 for business plan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>

- <span data-ttu-id="129e6-105">Pokud chcete zjistit verzi Office, kterou právě používáte, přečtěte si článek [o Office: jakou verzi Office](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)používám?.</span><span class="sxs-lookup"><span data-stu-id="129e6-105">To find the version of Office you are currently using, see [About Office: What version of Office am I using?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span></span>
- <span data-ttu-id="129e6-106">Pokud chcete zjistit Build, který chcete vrátit zpátky, přečtěte si článek [Historie aktualizací pro aplikace Microsoft 365 (uvedené podle data)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span><span class="sxs-lookup"><span data-stu-id="129e6-106">To determine the build you want to roll back to, see [Update history for Microsoft 365 Apps (listed by date)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span></span>
- <span data-ttu-id="129e6-107">Nakonfigurujte nastavení **TargetVersion** tak, aby se vrátilo ke staršímu buildu, a to tak, že se [vrátíte k dřívější verzi Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) nebo se [při používání sítě CDN (Office Content Delivery Network) přejímají aktualizace funkcí z pololetního kanálu](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span><span class="sxs-lookup"><span data-stu-id="129e6-107">Configure the **TargetVersion** setting to revert to the earlier build by using [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) or [Delay receiving feature updates from Semi-Annual Channel when using the Office Content Delivery Network (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span></span></br>
    <span data-ttu-id="129e6-108">Pokud je nastavená cílová verze, Office ji při příštím vyhledání aktualizací aktualizuje.</span><span class="sxs-lookup"><span data-stu-id="129e6-108">When the target version is set, Office updates to that version the next time it looks for updates.</span></span>