---
title: Automatické použití popisků citlivosti
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1737"
- "9000181"
ms.openlocfilehash: 8f316ad92ff31e28c3b3ffd25f25bd03ee159380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715158"
---
# <a name="auto-apply-sensitivity-labels"></a><span data-ttu-id="ed721-102">Automatické použití popisků citlivosti</span><span class="sxs-lookup"><span data-stu-id="ed721-102">Auto-apply sensitivity labels</span></span>

<span data-ttu-id="ed721-103">Popisky citlivosti můžou uživatelé ručně použít na obsah, nebo je můžete nakonfigurovat tak, aby se automaticky použily k obsahu.</span><span class="sxs-lookup"><span data-stu-id="ed721-103">Sensitivity labels can be manually applied to content by users, or you can configure them to be automatically applied to content.</span></span>

<span data-ttu-id="ed721-104">Automatické použití štítků s citlivostí odebere nutnost informovat uživatele o klasifikaci obsahu a o tom, že jim bude potřeba oznámení o konfiguraci zásad.</span><span class="sxs-lookup"><span data-stu-id="ed721-104">Automatically applying sensitivity labels removes the need to train users on how to classify content and the need to notify them of policy configurations.</span></span>

<span data-ttu-id="ed721-105">Pokud chcete popisky použít automaticky, je potřeba:</span><span class="sxs-lookup"><span data-stu-id="ed721-105">To apply labels automatically, the following is required:</span></span>

- <span data-ttu-id="ed721-106">Předplatné Azure Information Protection P2</span><span class="sxs-lookup"><span data-stu-id="ed721-106">Azure Information Protection P2 subscription</span></span>
- [<span data-ttu-id="ed721-107">Stažení a instalace klienta jednotného značení ochrany informací Azure</span><span class="sxs-lookup"><span data-stu-id="ed721-107">Download and install the Azure Information Protection unified labeling client</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

<span data-ttu-id="ed721-108">Pracujeme na nativní podpoře, která v budoucnu nevyžadují jednotné používání ochrany informací Azure.</span><span class="sxs-lookup"><span data-stu-id="ed721-108">We're working on native support that won't require the Azure Information Protection unified labeling client in the future.</span></span>

<span data-ttu-id="ed721-109">V současné době podporuje aktivní klient pro označení pouze systém Windows.</span><span class="sxs-lookup"><span data-stu-id="ed721-109">Currently, only Windows supports the unified labeling client.</span></span>  <span data-ttu-id="ed721-110">Funkce ještě není podporovaná na Macu, iOS a Androidu.</span><span class="sxs-lookup"><span data-stu-id="ed721-110">The feature is not yet supported on Mac, iOS and Android.</span></span>

<span data-ttu-id="ed721-111">Další informace o popisech citlivosti a jejich automatickém použití k obsahu najdete v tématech:</span><span class="sxs-lookup"><span data-stu-id="ed721-111">For more information on sensitivity labels and applying them automatically to content,  see:</span></span>

- [<span data-ttu-id="ed721-112">Základní informace o popisech citlivosti</span><span class="sxs-lookup"><span data-stu-id="ed721-112">Overview of sensitivity labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [<span data-ttu-id="ed721-113">Automatické použití popisku utajení u obsahu</span><span class="sxs-lookup"><span data-stu-id="ed721-113">Apply a sensitivity label to content automatically</span></span>](https://docs.microsoft.com/office365/securitycompliance/apply_sensitivity_label_automatically)