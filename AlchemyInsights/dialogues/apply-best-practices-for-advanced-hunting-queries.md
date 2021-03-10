---
title: Použití doporučených postupů pro pokročilé dotazy na hledání
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693345"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="4c7d1-102">Použití doporučených postupů pro pokročilé dotazy na hledání</span><span class="sxs-lookup"><span data-stu-id="4c7d1-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="4c7d1-103">Pokud chcete získat výsledky rychleji a vyhnout se časovým limitům při spouštění složitých dotazů, použijte tyto doporučené postupy:</span><span class="sxs-lookup"><span data-stu-id="4c7d1-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="4c7d1-104">Když zkoušíte nové dotazy, vždycky používejte limit, abyste nedocházelo k tomu, že by nedocházelo k příliš velkým sadám výsledků.</span><span class="sxs-lookup"><span data-stu-id="4c7d1-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="4c7d1-105">Můžete také `count` udělat počáteční vyhodnocení velikosti sady výsledků.</span><span class="sxs-lookup"><span data-stu-id="4c7d1-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="4c7d1-106">Nejdřív použijte filtry času.</span><span class="sxs-lookup"><span data-stu-id="4c7d1-106">Use time filters first.</span></span> <span data-ttu-id="4c7d1-107">V ideálním případě můžete dotazy omezit na sedm dní.</span><span class="sxs-lookup"><span data-stu-id="4c7d1-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="4c7d1-108">Na začátku dotazu hned za časovým filtrem přidejte filtry, u které se očekává, že se odebere většina dat.</span><span class="sxs-lookup"><span data-stu-id="4c7d1-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="4c7d1-109">Při hledání úplných tokenů použijte `has` operátor místo `contains` .</span><span class="sxs-lookup"><span data-stu-id="4c7d1-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="4c7d1-110">Vyhledávání v určitém sloupci místo ve všech sloupcích</span><span class="sxs-lookup"><span data-stu-id="4c7d1-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="4c7d1-111">Při spojování tabulek nejdřív určete tabulku s menším počtem řádků.</span><span class="sxs-lookup"><span data-stu-id="4c7d1-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="4c7d1-112">`project` jenom potřebné sloupce z tabulek, které jste připojili.</span><span class="sxs-lookup"><span data-stu-id="4c7d1-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="4c7d1-113">Další informace najdete v doporučených [postupech pro pokročilé dotazy k hledání.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="4c7d1-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
