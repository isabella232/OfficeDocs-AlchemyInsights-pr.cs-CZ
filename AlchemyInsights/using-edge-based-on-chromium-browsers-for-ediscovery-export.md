---
title: Použití Microsoft Edge založeného na prohlížečích Chromium pro export Ediscovery
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834364"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="00f14-102">Použití Microsoft Edge založeného na prohlížečích Chromium pro export Ediscovery</span><span class="sxs-lookup"><span data-stu-id="00f14-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="00f14-103">Kvůli nedávné změně už prohlížeče Microsoft Edge nebudou mít ve výchozím nastavení povolenou podporu ClickOnce.</span><span class="sxs-lookup"><span data-stu-id="00f14-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="00f14-104">Pokud chcete nástroj Microsoft 365 eDiscovery Exportovat dál používat, budete muset buď používat Microsoft Internet Explorer, nebo povolit podporu ClickOnce v Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="00f14-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="00f14-105">Povolení podpory ClickOnce v Microsoft Edge na základě chromu:</span><span class="sxs-lookup"><span data-stu-id="00f14-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="00f14-106">V prohlížeči Microsoft Edge přejděte na edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="00f14-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="00f14-107">U možnosti Podpora ClickOnce změňte hodnotu z **výchozího** nebo **zakázaného** na **Povoleno**.</span><span class="sxs-lookup"><span data-stu-id="00f14-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="00f14-108">V dolní části okna prohlížeče vyberte **Restartovat.**</span><span class="sxs-lookup"><span data-stu-id="00f14-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="00f14-109">Změna se projeví po restartování Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="00f14-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="00f14-110">Informace o tomto postupu a postupu pro instalaci nástroje pro export najdete v tématu Export [výsledků hledání obsahu.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="00f14-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>