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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="3bff2-102">"Požadované Alchymie Záhlaví H1, H2 nefungují."</span><span class="sxs-lookup"><span data-stu-id="3bff2-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="3bff2-103">Doporučené postupy a pokyny pro vytváření alchymie:</span><span class="sxs-lookup"><span data-stu-id="3bff2-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="3bff2-104">**Nehnožte Alchymie Insights ve složkách**- to zlomí strukturu url.</span><span class="sxs-lookup"><span data-stu-id="3bff2-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="3bff2-105">Prověřujeme, jak to napravit.</span><span class="sxs-lookup"><span data-stu-id="3bff2-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="3bff2-106">Soubory ve složce **AlchymieInsights** by měly mít názvy souborů s malými písmeny s pomlčkami pro mezery ex.</span><span class="sxs-lookup"><span data-stu-id="3bff2-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="3bff2-107">***jak povolit blokování soudních sporů***.</span><span class="sxs-lookup"><span data-stu-id="3bff2-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="3bff2-108">Do pole ms.custom zahrňte ID pravidla nebo ID bloku z [portálu Alchymie Partner.](https://alchemyportal.azurewebsites.net)</span><span class="sxs-lookup"><span data-stu-id="3bff2-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="3bff2-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="3bff2-109">ex.</span></span> <span data-ttu-id="3bff2-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="3bff2-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="3bff2-111">Jako šablonu použijte zbývající metadata v horní části tohoto souboru.</span><span class="sxs-lookup"><span data-stu-id="3bff2-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="3bff2-112">Na [portálu Alchemy Partner](https://alchemyportal.azurewebsites.net)přejděte do části **Název customer insightu a** použijte ji jako výchozí bod pro titul H1 pro přehled.</span><span class="sxs-lookup"><span data-stu-id="3bff2-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="3bff2-113">Alchymie Insights musí mít pouze jeden H1 na vrcholu, nebo se zlomí ve výrobě.</span><span class="sxs-lookup"><span data-stu-id="3bff2-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="3bff2-114">H2s nevykreslují buď tak použít **tučné** nebo jiné konvence znamenat samostatné oddíly.</span><span class="sxs-lookup"><span data-stu-id="3bff2-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="3bff2-115">Dále vyplňte základní text pomocí materiálu konceptu v části Customer Insights na stránce Pravidlo alchymie.</span><span class="sxs-lookup"><span data-stu-id="3bff2-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="3bff2-116">Seznamy s odrážkami jsou v pořádku</span><span class="sxs-lookup"><span data-stu-id="3bff2-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="3bff2-117">Také číslované seznamy</span><span class="sxs-lookup"><span data-stu-id="3bff2-117">Numbered lists too</span></span>
    1. <span data-ttu-id="3bff2-118">**Tučné** a *kurzíva* jsou a-ok</span><span class="sxs-lookup"><span data-stu-id="3bff2-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="3bff2-119">Odkazy by měly být vždy buď **"odkazy na web" / externí** nebo **hluboké odkazy na prvky uživatelského rozhraní**, nikoli interní odkazy.</span><span class="sxs-lookup"><span data-stu-id="3bff2-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="3bff2-120">Obrázky nejsou v tuto chvíli oficiálně podporovány, ale jsou v plánu.</span><span class="sxs-lookup"><span data-stu-id="3bff2-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="3bff2-121">A to už je opravdu trochu moc dlouhé.</span><span class="sxs-lookup"><span data-stu-id="3bff2-121">And this is really already a bit too long.</span></span> <span data-ttu-id="3bff2-122">Osvědčeným postupem je asi 400 znaků ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="3bff2-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="3bff2-123">Jakmile je obsah připraven, vytáhněte jej do živé větve.</span><span class="sxs-lookup"><span data-stu-id="3bff2-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="3bff2-124">Potom přejděte na [portál Alchymie Partner](https://alchemyportal.azurewebsites.net) a zadejte název souboru do pole url.</span><span class="sxs-lookup"><span data-stu-id="3bff2-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 