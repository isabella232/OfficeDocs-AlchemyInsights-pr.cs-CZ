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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930126"
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
