---
title: 1490 – řešení potíží – eDiscovery – chyby
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277835"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="dc273-102">Řešení chyb při hledání obsahu</span><span class="sxs-lookup"><span data-stu-id="dc273-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="dc273-103">Máte problémy s vyhledáváním obsahu nebo se selháním při exportu výsledků hledání?</span><span class="sxs-lookup"><span data-stu-id="dc273-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="dc273-104">Při provádění hledání se například zobrazuje následující:</span><span class="sxs-lookup"><span data-stu-id="dc273-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="dc273-105">Chyby CS008 nebo CS012</span><span class="sxs-lookup"><span data-stu-id="dc273-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="dc273-106">Chyby při obsazení nebo vypršení časového limitu serveru</span><span class="sxs-lookup"><span data-stu-id="dc273-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="dc273-107">Došlo k chybě aplikace.</span><span class="sxs-lookup"><span data-stu-id="dc273-107">Application error occurred</span></span>

<span data-ttu-id="dc273-108">Nebo při vyhledávání nebo exportu výsledků z velkého počtu poštovních schránek (přes 100 000 poštovních schránek) se zobrazují chyby při exportu?</span><span class="sxs-lookup"><span data-stu-id="dc273-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="dc273-109">U těchto typů chyb opakujte hledání u neúspěšných umístění obsahu.</span><span class="sxs-lookup"><span data-stu-id="dc273-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="dc273-110">Další informace najdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="dc273-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="dc273-111">Pokud exportujete víc než 100K poštovních schránek, budete muset ke stažení výsledků exportu použít následující PowerShell:  [Export výsledků z víc než 100K poštovní schránky](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="dc273-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
