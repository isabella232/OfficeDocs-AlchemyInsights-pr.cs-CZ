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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="77da8-102">"Povinné záhlaví Alchemy H1, H2's nefunguje."</span><span class="sxs-lookup"><span data-stu-id="77da8-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="77da8-103">Doporučené postupy a pokyny pro vytváření Alchemy:</span><span class="sxs-lookup"><span data-stu-id="77da8-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="77da8-104">**Do složek nevnořit Alchemy přehledy**– toto přeruší strukturu adres URL.</span><span class="sxs-lookup"><span data-stu-id="77da8-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="77da8-105">Pracujeme na vyřešení tohoto řešení.</span><span class="sxs-lookup"><span data-stu-id="77da8-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="77da8-106">Soubory ve složce **AlchemyInsights** by měly obsahovat názvy souborů s malými písmeny s pomlčkami pro mezery.</span><span class="sxs-lookup"><span data-stu-id="77da8-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="77da8-107">***postupy – povolení-soudní spory***</span><span class="sxs-lookup"><span data-stu-id="77da8-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="77da8-108">Do pole MS. Custom zadejte ID pravidla nebo ID bloku z [portálu Alchemy partnera](https://alchemyportal.azurewebsites.net) .</span><span class="sxs-lookup"><span data-stu-id="77da8-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="77da8-109">Příklad.</span><span class="sxs-lookup"><span data-stu-id="77da8-109">ex.</span></span> <span data-ttu-id="77da8-110">***MS. vlastní: 100021***</span><span class="sxs-lookup"><span data-stu-id="77da8-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="77da8-111">V horní části tohoto souboru použijte zbývající metadata jako šablonu.</span><span class="sxs-lookup"><span data-stu-id="77da8-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="77da8-112">Na [portálu Alchemy partnera](https://alchemyportal.azurewebsites.net)přejděte na téma popis **zákazníka – přehled:** a použijte ho jako výchozí bod pro váš název H1 pro přehled.</span><span class="sxs-lookup"><span data-stu-id="77da8-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="77da8-113">Alchemy přehledy musí mít v horní části jenom jeden H1 nebo se budou přerušit ve výrobě.</span><span class="sxs-lookup"><span data-stu-id="77da8-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="77da8-114">H2s nevykreslují, takže nepoužívejte k označení samostatných oddílů **tučné** nebo jiné zvyklosti.</span><span class="sxs-lookup"><span data-stu-id="77da8-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="77da8-115">Potom vyplňte základní text pomocí konceptu materiál v části zákaznické přehledy na stránce pravidlo Alchemy.</span><span class="sxs-lookup"><span data-stu-id="77da8-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="77da8-116">Seznamy s odrážkami jsou přesné</span><span class="sxs-lookup"><span data-stu-id="77da8-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="77da8-117">Číslované seznamy</span><span class="sxs-lookup"><span data-stu-id="77da8-117">Numbered lists too</span></span>
    1. <span data-ttu-id="77da8-118">**Tučné písmo** a *kurzíva* jsou a – OK</span><span class="sxs-lookup"><span data-stu-id="77da8-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="77da8-119">Odkazy by měly vždy být **"odkazy na web"/External** nebo **hluboké odkazy na prvky uživatelského rozhraní**, ne interní odkazy.</span><span class="sxs-lookup"><span data-stu-id="77da8-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="77da8-120">Obrázky nejsou v současné době oficiálně podporovány, ale je to v plánu.</span><span class="sxs-lookup"><span data-stu-id="77da8-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="77da8-121">A to je opravdu příliš dlouho.</span><span class="sxs-lookup"><span data-stu-id="77da8-121">And this is really already a bit too long.</span></span> <span data-ttu-id="77da8-122">Osvědčené postupy jsou přibližně 400 znaků---------------------------------</span><span class="sxs-lookup"><span data-stu-id="77da8-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="77da8-123">Jakmile je váš obsah připravený, vytáhněte ho do živé větvení.</span><span class="sxs-lookup"><span data-stu-id="77da8-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="77da8-124">Pak přejděte na [portál partnera Alchemy](https://alchemyportal.azurewebsites.net) a zadejte název souboru do pole URL.</span><span class="sxs-lookup"><span data-stu-id="77da8-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 