---
title: nejlepší je název souboru
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
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312818"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Required Alchemy Header H1, H2's don't work".
Doporučené postupy a pokyny pro vytváření alchymií:

1. **Vnořovat Alchemy Přehledy do složek**– tím se přeruší struktura adresy URL. Hledáme řešení tohoto řešení.
1. Soubory ve **složce AlchemyInsights** by měly mít malé názvy souborů s pomlčkami pro mezery ex. **_how-to-enable-litigation-hold_**.
    1. Do pole ms.custom zadejte ID pravidla nebo ID bucketu z [portálu Alchemy Partner.](https://alchemyportal.azurewebsites.net) ex. ***ms.custom: 100021***
1. Jako šablonu použijte zbytek metadat v horní části tohoto souboru.
1. Na portálu [Alchemy Partner přejděte](https://alchemyportal.azurewebsites.net)dolů do oddílu Customer Insight Title (Název customer **insightu):** a použijte ho jako výchozí bod pro název H1 pro přehled. 

**Poznámka:** Alchemy Přehledy musí mít nahoře jenom jeden H1 nebo se přeruší v produkčním prostředí. H2s se nevykreslují, takže k označení samostatných oddílů použijte tučné písmo nebo jiné konvence. 
1. Potom vyplňte hlavní text pomocí konceptu v části Customer Insights stránky Alchemy Rule (Pravidlo alchymie).
    1. Seznamy s odrážkami jsou v pořádku.
    1. Číslování seznamů
    1. **Tučné** písmo a *kurzíva* jsou v pořádku.
    1. Odkazy by měly být vždy **buď "odkazy na web"/externí** nebo **odkazy na** prvky uživatelského rozhraní , ne interní odkazy.
    1. Obrázky nejsou v tuto chvíli oficiálně podporované, ale jsou v plánu.

A už je to moc dlouho. Osvědčený postup je asi 400 znaků ---------------------------------

Až bude obsah připravený, přetáhněte ho do živé větve. Potom přejděte na portál [Alchemy Partner a](https://alchemyportal.azurewebsites.net) zadejte název souboru do pole url. 