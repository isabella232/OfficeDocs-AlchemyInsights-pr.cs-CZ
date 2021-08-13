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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918888"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Required Alchemy Header H1, H2's don't work".
Doporučené postupy a pokyny pro vytváření alchymií:

1. **Ne vnořovat Alchemy Přehledy do složek**– tím se struktura adresy URL přeruší. Hledáme řešení tohoto řešení.
1. Soubory ve **složce AlchemyInsights** by měly mít malé názvy souborů s pomlčkami pro mezery ex. **_how-to-enable-litigation-hold_**.
    1. Do pole ms.custom zadejte ID pravidla nebo ID bucketu z [portálu Alchemy Partner](https://alchemyportal.azurewebsites.net) Portal. ex. ***ms.custom: 100021***
1. Jako šablonu použijte zbytek metadat v horní části tohoto souboru.
1. Na portálu [Alchemy Partner přejděte](https://alchemyportal.azurewebsites.net)dolů do oddílu Customer Insight Title (Název customer **insightu):** a použijte ho jako výchozí bod pro název H1 pro přehled. 
    > [!NOTE]
    > Alchemy Přehledy musí mít nahoře jenom jeden H1, nebo se přeruší v produkčním prostředí. H2s se nevykreslují, takže k označení samostatných oddílů použijte tučné písmo nebo jiné konvence. 
1. Potom vyplňte hlavní text pomocí konceptu v části Customer Insights stránky Alchemy Rule (Pravidlo alchymie).
    1. Seznamy s odrážkami jsou v pořádku.
    1. Číslování seznamů
    1. **Tučné** písmo a *kurzíva* jsou v pořádku.
    1. Odkazy by měly být vždy **buď "odkazy na web"/externí** nebo **odkazy na** prvky uživatelského rozhraní , ne interní odkazy.
    1. Obrázky nejsou v tuto chvíli oficiálně podporované, ale jsou v plánu.

A už je to moc dlouho. Osvědčený postup je asi 400 znaků ---------------------------------

Až bude obsah připravený, přetáhněte ho do živé větve. Potom přejděte na portál [Alchemy Partner a](https://alchemyportal.azurewebsites.net) zadejte název souboru do pole url. 