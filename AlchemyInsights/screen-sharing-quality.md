---
title: Kvalita sdílení obrazovky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/26/2021
ms.locfileid: "52124904"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="5352c-102">Kvalita sdílení obrazovky</span><span class="sxs-lookup"><span data-stu-id="5352c-102">Screen sharing quality</span></span>

<span data-ttu-id="5352c-103">Ve většině případů se problémy se sdílením obrazovky s kvalitou z klientské strany zkují na omezenou šířku pásma.</span><span class="sxs-lookup"><span data-stu-id="5352c-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="5352c-104">Pokud šířka pásma není omezená, Teams optimalizuje kvalitu médií, včetně rozlišení videa s rozlišením až 1 080p, až 30fps pro video a 15fps pro obsah a zvuku s vysokou věrností.</span><span class="sxs-lookup"><span data-stu-id="5352c-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="5352c-105">Teams je vždy konzervativní na využití šířky pásma a může poskytovat hd kvalitu videa za méně než 1,2 Mb/s.</span><span class="sxs-lookup"><span data-stu-id="5352c-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="5352c-106">Skutečná spotřeba šířky pásma v každém audiovizuálním hovoru nebo schůzce se liší v závislosti na faktorech, jako je rozložení videa, rozlišení videa a snímky videa za sekundu.</span><span class="sxs-lookup"><span data-stu-id="5352c-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="5352c-107">Pokud je dostupná větší šířka pásma, zvýší se kvalita a využití, aby bylo možné zajistit nejlepší možnosti.</span><span class="sxs-lookup"><span data-stu-id="5352c-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="5352c-108">Tato tabulka popisuje, jak Teams používá šířku pásma:</span><span class="sxs-lookup"><span data-stu-id="5352c-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="5352c-109">**Scénáře šířky pásma(nahoru/dolů)**</span><span class="sxs-lookup"><span data-stu-id="5352c-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="5352c-110">30 kb/s audiohovory mezi dvěma hovory</span><span class="sxs-lookup"><span data-stu-id="5352c-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="5352c-111">130 kbps Peer-to-peer audio calling and screen sharing</span><span class="sxs-lookup"><span data-stu-id="5352c-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="5352c-112">Videohovory 360p při 30fps s rychlostí 500 kb/s</span><span class="sxs-lookup"><span data-stu-id="5352c-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="5352c-113">1,2 Mb/s Videohovory v hd kvalitě s rozlišením HD 720p při 30fps</span><span class="sxs-lookup"><span data-stu-id="5352c-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="5352c-114">Videohovory s rychlostí 1,5 Mb/s v hd kvalitě s rozlišením HD 1080p při 30fps</span><span class="sxs-lookup"><span data-stu-id="5352c-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="5352c-115">500kbps/1Mbps Group Video calling</span><span class="sxs-lookup"><span data-stu-id="5352c-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="5352c-116">Videohovory skupiny HD s rychlostí 1 Mb/s (540p videa na obrazovce 1080p)</span><span class="sxs-lookup"><span data-stu-id="5352c-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="5352c-117">Další informace najdete v tématu Příprava sítě vaší [organizace na Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span><span class="sxs-lookup"><span data-stu-id="5352c-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>