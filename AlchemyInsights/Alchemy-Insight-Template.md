---
title: stejné jako název souboru je nejlepší
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750963"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Požadované Alchymie Záhlaví H1, H2 nefungují."
Doporučené postupy a pokyny pro vytváření alchymie:

1. **Nehnožte Alchymie Insights ve složkách**- to zlomí strukturu url. Prověřujeme, jak to napravit.
1. Soubory ve složce **AlchymieInsights** by měly mít názvy souborů s malými písmeny s pomlčkami pro mezery ex. ***jak povolit blokování soudních sporů***.
    1. Do pole ms.custom zahrňte ID pravidla nebo ID bloku z [portálu Alchymie Partner.](https://alchemyportal.azurewebsites.net) Ex. ***ms.custom: 100021***
1. Jako šablonu použijte zbývající metadata v horní části tohoto souboru.
1. Na [portálu Alchemy Partner](https://alchemyportal.azurewebsites.net)přejděte do části **Název customer insightu a** použijte ji jako výchozí bod pro titul H1 pro přehled. 
    > [!NOTE]
    > Alchymie Insights musí mít pouze jeden H1 na vrcholu, nebo se zlomí ve výrobě. H2s nevykreslují buď tak použít **tučné** nebo jiné konvence znamenat samostatné oddíly.
1. Dále vyplňte základní text pomocí materiálu konceptu v části Customer Insights na stránce Pravidlo alchymie.
    1. Seznamy s odrážkami jsou v pořádku
    1. Také číslované seznamy
    1. **Tučné** a *kurzíva* jsou a-ok
    1. Odkazy by měly být vždy buď **"odkazy na web" / externí** nebo **hluboké odkazy na prvky uživatelského rozhraní**, nikoli interní odkazy.
    1. Obrázky nejsou v tuto chvíli oficiálně podporovány, ale jsou v plánu.

A to už je opravdu trochu moc dlouhé. Osvědčeným postupem je asi 400 znaků ---------------------------------

Jakmile je obsah připraven, vytáhněte jej do živé větve. Potom přejděte na [portál Alchymie Partner](https://alchemyportal.azurewebsites.net) a zadejte název souboru do pole url. 