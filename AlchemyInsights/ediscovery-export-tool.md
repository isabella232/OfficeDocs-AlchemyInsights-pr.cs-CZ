---
title: Nástroj pro export eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814581"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="47b49-102">Nemůžete nainstalovat nebo spustit nástroj pro export eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="47b49-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="47b49-103">Pokud nemůžete nainstalovat nebo spustit nástroj pro export eDiscovery a stáhnout výsledky hledání, podívejte se na následující věci:</span><span class="sxs-lookup"><span data-stu-id="47b49-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="47b49-104">Počítač, který používáte, splňuje tyto předpoklady:</span><span class="sxs-lookup"><span data-stu-id="47b49-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="47b49-105">32bitová nebo 64bitová verze Windows 7 a novějších verzí</span><span class="sxs-lookup"><span data-stu-id="47b49-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="47b49-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="47b49-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="47b49-107">Podporovaný prohlížeč:</span><span class="sxs-lookup"><span data-stu-id="47b49-107">A supported browser:</span></span>

  - <span data-ttu-id="47b49-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="47b49-108">Microsoft Edge</span></span>

    <span data-ttu-id="47b49-109">Nebo</span><span class="sxs-lookup"><span data-stu-id="47b49-109">Or</span></span>

  - <span data-ttu-id="47b49-110">Internet Explorer 10 a novější verze</span><span class="sxs-lookup"><span data-stu-id="47b49-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="47b49-111">Jiné prohlížeče, jako je Google Chrome nebo Mozilla Firefox, nejsou podporované.</span><span class="sxs-lookup"><span data-stu-id="47b49-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="47b49-112">Vaše organizace se může připojit k koncovému bodu v Azure, což je **\* .blob.core.windows.net** (zástupný znak představuje jedinečný identifikátor exportu).</span><span class="sxs-lookup"><span data-stu-id="47b49-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="47b49-113">V Centru dodržování předpisů zabezpečení Microsoftu 365 máte přiřazenou roli &amp; Exportovat.</span><span class="sxs-lookup"><span data-stu-id="47b49-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="47b49-114">Ve výchozím nastavení je tato role přiřazená jenom skupině rolí Správce eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="47b49-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="47b49-115">Viz [Přiřazení oprávnění k eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="47b49-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="47b49-116">Další informace najdete v článku [Export výsledků hledání obsahu](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="47b49-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="47b49-117">Pokud exportujete víc než 100 tisíc poštovních schránek, budete muset stáhnout výsledky exportu pomocí následujícího PowerShellu: Export výsledků z více než  [100 tisíc poštovních schránek](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="47b49-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>