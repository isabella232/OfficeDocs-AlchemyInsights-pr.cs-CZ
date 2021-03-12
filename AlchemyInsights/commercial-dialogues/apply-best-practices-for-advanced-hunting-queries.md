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
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Použití osvědčených postupů pro pokročilé lovecké dotazy

Pokud chcete získat výsledky rychleji a vyhnout se časovým limitům při spouštění složitých dotazů, použijte tyto doporučené postupy:

- Při pokusu o nové dotazy vždy použijte limit, abyste nedocházelo k extrémně velkým sadám výsledků. Můžete také provést počáteční posouzení velikosti `count` sady výsledků.
- Nejdřív použijte filtry času. V ideálním případě omezte dotazy na sedm dní.
- Na začátku dotazu hned za časovým filtrem přidejte filtry, které mají většinu dat odebrat.
- Když hledáte úplné tokeny, použijte `has` operátor místo `contains` .
- Spusťte hledání na určitém sloupci, ne napříč všemi sloupci.
- Při spojování tabulek nejdřív určete tabulku s menším počtem řádků.
- `project` pouze potřebné sloupce z tabulek, které jste připojili.

Další informace najdete v tématu Doporučené postupy pro rozšířené [lovecké dotazy](https://go.microsoft.com/fwlink/?linkid=2144812).
