---
title: Nástroj pro export eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277926"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="0ac46-102">Nejde nainstalovat nebo spustit nástroj pro export eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="0ac46-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="0ac46-103">Pokud se vám nedaří nainstalovat nebo spustit nástroj pro export eDiscovery ke stažení výsledků hledání, podívejte se na tyto věci:</span><span class="sxs-lookup"><span data-stu-id="0ac46-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="0ac46-104">Počítač, který používáte, splňuje tyto předpoklady:</span><span class="sxs-lookup"><span data-stu-id="0ac46-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="0ac46-105">32 nebo 64 verze Windows 7 a novější verze</span><span class="sxs-lookup"><span data-stu-id="0ac46-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="0ac46-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="0ac46-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="0ac46-107">Podporovaný prohlížeč:</span><span class="sxs-lookup"><span data-stu-id="0ac46-107">A supported browser:</span></span>

  - <span data-ttu-id="0ac46-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0ac46-108">Microsoft Edge</span></span>

    <span data-ttu-id="0ac46-109">Nebo</span><span class="sxs-lookup"><span data-stu-id="0ac46-109">Or</span></span>

  - <span data-ttu-id="0ac46-110">Internet Explorer 10 a novější verze</span><span class="sxs-lookup"><span data-stu-id="0ac46-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="0ac46-111">Jiné prohlížeče, například Google Chrome a Mozilla Firefox, nejsou podporované.</span><span class="sxs-lookup"><span data-stu-id="0ac46-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="0ac46-112">Vaše organizace se může připojit ke koncovému bodu v Azure, což je \*\* \* . blob.Core.Windows.NET\*\* (zástupný znak představuje jedinečný identifikátor úlohy exportu).</span><span class="sxs-lookup"><span data-stu-id="0ac46-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="0ac46-113">Přiřadili jste roli exportu v centru zabezpečení Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="0ac46-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="0ac46-114">Ve výchozím nastavení je tato role přiřazena jenom skupině role správce eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="0ac46-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="0ac46-115">Viz [přiřazení oprávnění eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="0ac46-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="0ac46-116">Další informace najdete v článku [Export výsledků hledání obsahu](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="0ac46-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="0ac46-117">Pokud exportujete víc než 100K poštovních schránek, budete muset ke stažení výsledků exportu použít následující PowerShell:  [Export výsledků z víc než 100K poštovní schránky](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="0ac46-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>