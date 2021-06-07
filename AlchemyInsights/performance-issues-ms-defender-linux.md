---
title: Problémy s výkonem pro Microsoft Defender pro koncový bod v Linuxu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793638"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="f9acf-102">Problémy s výkonem pro Microsoft Defender pro koncový bod v Linuxu</span><span class="sxs-lookup"><span data-stu-id="f9acf-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="f9acf-103">Tento článek vás provede kroky identifikace problémů s výkonem pro Microsoft Defender pro koncový bod v Linuxu.</span><span class="sxs-lookup"><span data-stu-id="f9acf-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="f9acf-104">Nejdřív je důležité ověřit, jestli je problém vyřešený v [nejnovější verzi](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="f9acf-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="f9acf-105">Pokud chcete zahájit vyšetřování, podívejte se na článek Řešení problémů s [výkonem v Microsoft Defenderu pro koncový bod v Linuxu](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="f9acf-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="f9acf-106">Vyloučení</span><span class="sxs-lookup"><span data-stu-id="f9acf-106">Exclusions</span></span>

<span data-ttu-id="f9acf-107">Vyloučení můžou pomoct zmírnit problémy s výkonem.</span><span class="sxs-lookup"><span data-stu-id="f9acf-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="f9acf-108">Než začnete, zkontrolujte si vyloučení, aby bylo známé a zdokumentované jakékoli další riziko.</span><span class="sxs-lookup"><span data-stu-id="f9acf-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="f9acf-109">Další informace najdete v tématu Konfigurace a ověření vyloučení pro [Microsoft Defender pro koncový bod v Linuxu](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="f9acf-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="f9acf-110">Pokud máte více souborů & složek, které chcete vyloučit, a všechny jsou na stejném přípojných bodech, může být jednodušší vyřadit přípojný bod.</span><span class="sxs-lookup"><span data-stu-id="f9acf-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="f9acf-111">Počínaje únorovou verzí 101.22.80 můžete vyloučit celý mountpoint.</span><span class="sxs-lookup"><span data-stu-id="f9acf-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="f9acf-112">Pokud je například přípojný bod /mnt/backup, můžete do seznamu vyloučení přidat /mnt/backup spuštěním tohoto příkazu:</span><span class="sxs-lookup"><span data-stu-id="f9acf-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="f9acf-113">**Poznámka:** Přidáním výjimek se zvyšuje riziko, že malware nebude detekován, a mělo by se s ním zacházet a implementovat opatrně.</span><span class="sxs-lookup"><span data-stu-id="f9acf-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="f9acf-114">Potřebujete pomoct?</span><span class="sxs-lookup"><span data-stu-id="f9acf-114">Need Help?</span></span>

<span data-ttu-id="f9acf-115">Abyste vám pomohli co nejefektivnějším způsobem, shromážděte diagnostická data před otevřením případu podpory.</span><span class="sxs-lookup"><span data-stu-id="f9acf-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
