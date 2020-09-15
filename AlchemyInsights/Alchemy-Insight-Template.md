---
title: nejvhodnější je název souboru.
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664127"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Povinné záhlaví Alchemy H1, H2's nefunguje."
Doporučené postupy a pokyny pro vytváření Alchemy:

1. **Do složek nevnořit Alchemy přehledy**– toto přeruší strukturu adres URL. Pracujeme na vyřešení tohoto řešení.
1. Soubory ve složce **AlchemyInsights** by měly obsahovat názvy souborů s malými písmeny s pomlčkami pro mezery. ***postupy – povolení-soudní spory***
    1. Do pole MS. Custom zadejte ID pravidla nebo ID bloku z [portálu Alchemy partnera](https://alchemyportal.azurewebsites.net) . Příklad. ***MS. vlastní: 100021***
1. V horní části tohoto souboru použijte zbývající metadata jako šablonu.
1. Na [portálu Alchemy partnera](https://alchemyportal.azurewebsites.net)přejděte na téma popis **zákazníka – přehled:** a použijte ho jako výchozí bod pro váš název H1 pro přehled. 
    > [!NOTE]
    > Alchemy přehledy musí mít v horní části jenom jeden H1 nebo se budou přerušit ve výrobě. H2s nevykreslují, takže nepoužívejte k označení samostatných oddílů **tučné** nebo jiné zvyklosti.
1. Potom vyplňte základní text pomocí konceptu materiál v části zákaznické přehledy na stránce pravidlo Alchemy.
    1. Seznamy s odrážkami jsou přesné
    1. Číslované seznamy
    1. **Tučné písmo** a *kurzíva* jsou a – OK
    1. Odkazy by měly vždy být **"odkazy na web"/External** nebo **hluboké odkazy na prvky uživatelského rozhraní**, ne interní odkazy.
    1. Obrázky nejsou v současné době oficiálně podporovány, ale je to v plánu.

A to je opravdu příliš dlouho. Osvědčené postupy jsou přibližně 400 znaků---------------------------------

Jakmile je váš obsah připravený, vytáhněte ho do živé větvení. Pak přejděte na [portál partnera Alchemy](https://alchemyportal.azurewebsites.net) a zadejte název souboru do pole URL. 