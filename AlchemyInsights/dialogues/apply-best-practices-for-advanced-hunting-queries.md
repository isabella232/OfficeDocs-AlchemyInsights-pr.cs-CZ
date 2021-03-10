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
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Použití doporučených postupů pro pokročilé dotazy na hledání

Pokud chcete získat výsledky rychleji a vyhnout se časovým limitům při spouštění složitých dotazů, použijte tyto doporučené postupy:

- Když zkoušíte nové dotazy, vždycky používejte limit, abyste nedocházelo k tomu, že by nedocházelo k příliš velkým sadám výsledků. Můžete také `count` udělat počáteční vyhodnocení velikosti sady výsledků.
- Nejdřív použijte filtry času. V ideálním případě můžete dotazy omezit na sedm dní.
- Na začátku dotazu hned za časovým filtrem přidejte filtry, u které se očekává, že se odebere většina dat.
- Při hledání úplných tokenů použijte `has` operátor místo `contains` .
- Vyhledávání v určitém sloupci místo ve všech sloupcích
- Při spojování tabulek nejdřív určete tabulku s menším počtem řádků.
- `project` jenom potřebné sloupce z tabulek, které jste připojili.

Další informace najdete v doporučených [postupech pro pokročilé dotazy k hledání.](https://go.microsoft.com/fwlink/?linkid=2144812)
