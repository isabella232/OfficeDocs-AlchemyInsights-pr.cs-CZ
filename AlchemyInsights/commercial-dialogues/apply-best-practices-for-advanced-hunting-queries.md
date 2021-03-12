---
title: Použití osvědčených postupů pro pokročilé lovecké dotazy
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744608"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="13a14-102">Použití osvědčených postupů pro pokročilé lovecké dotazy</span><span class="sxs-lookup"><span data-stu-id="13a14-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="13a14-103">Pokud chcete získat výsledky rychleji a vyhnout se časovým limitům při spouštění složitých dotazů, použijte tyto doporučené postupy:</span><span class="sxs-lookup"><span data-stu-id="13a14-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="13a14-104">Při pokusu o nové dotazy vždy použijte limit, abyste nedocházelo k extrémně velkým sadám výsledků.</span><span class="sxs-lookup"><span data-stu-id="13a14-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="13a14-105">Můžete také provést počáteční posouzení velikosti `count` sady výsledků.</span><span class="sxs-lookup"><span data-stu-id="13a14-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="13a14-106">Nejdřív použijte filtry času.</span><span class="sxs-lookup"><span data-stu-id="13a14-106">Use time filters first.</span></span> <span data-ttu-id="13a14-107">V ideálním případě omezte dotazy na sedm dní.</span><span class="sxs-lookup"><span data-stu-id="13a14-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="13a14-108">Na začátku dotazu hned za časovým filtrem přidejte filtry, které mají většinu dat odebrat.</span><span class="sxs-lookup"><span data-stu-id="13a14-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="13a14-109">Když hledáte úplné tokeny, použijte `has` operátor místo `contains` .</span><span class="sxs-lookup"><span data-stu-id="13a14-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="13a14-110">Spusťte hledání na určitém sloupci, ne napříč všemi sloupci.</span><span class="sxs-lookup"><span data-stu-id="13a14-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="13a14-111">Při spojování tabulek nejdřív určete tabulku s menším počtem řádků.</span><span class="sxs-lookup"><span data-stu-id="13a14-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="13a14-112">`project` pouze potřebné sloupce z tabulek, které jste připojili.</span><span class="sxs-lookup"><span data-stu-id="13a14-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="13a14-113">Další informace najdete v tématu Doporučené postupy pro rozšířené [lovecké dotazy](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="13a14-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
