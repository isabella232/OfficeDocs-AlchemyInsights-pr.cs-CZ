---
title: Omezení SharePointu Online na klasický režim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751415"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="255d9-102">Omezení SharePointu Online na klasický režim</span><span class="sxs-lookup"><span data-stu-id="255d9-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="255d9-103">Některé organizace ještě vyžadují klasický režim.</span><span class="sxs-lookup"><span data-stu-id="255d9-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="255d9-104">Přestože neplánujete odebrání klasického režimu na podrobné úrovni, není už možné omezit celou organizaci (tenanta) na klasický režim pro seznamy a knihovny.</span><span class="sxs-lookup"><span data-stu-id="255d9-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="255d9-105">Správce bude mít následující možnosti pro správu jednotlivých seznamů a knihoven v klasickém režimu pomocí podrobných přepínačů pro výslovný nesouhlas, které poskytujeme na následujících úrovních:</span><span class="sxs-lookup"><span data-stu-id="255d9-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="255d9-106">kolekce webů</span><span class="sxs-lookup"><span data-stu-id="255d9-106">site collection</span></span>
- <span data-ttu-id="255d9-107">návštěvníků</span><span class="sxs-lookup"><span data-stu-id="255d9-107">site</span></span>
- <span data-ttu-id="255d9-108">výpis</span><span class="sxs-lookup"><span data-stu-id="255d9-108">list</span></span>
- <span data-ttu-id="255d9-109">knihovny</span><span class="sxs-lookup"><span data-stu-id="255d9-109">library</span></span>

<span data-ttu-id="255d9-110">Navíc seznamy, které používají určité funkce a přizpůsobení, se pořád budou automaticky přepínat do klasického režimu.</span><span class="sxs-lookup"><span data-stu-id="255d9-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="255d9-111">Zahájení 1. dubna 2019 se proces zakázání výslovného souhlasu na úrovni tenanta mimo moderní seznam a knihovny zahájí a pokračuje do 31 2019.</span><span class="sxs-lookup"><span data-stu-id="255d9-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="255d9-112">Seznamy a knihovny, které jsou v klasickém režimu jako výsledek výslovného souhlasu tenanta, se automaticky posunou na moderní.</span><span class="sxs-lookup"><span data-stu-id="255d9-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="255d9-113">Pokud vyžadujete klasický režim, podívejte se na [tady další informace a](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) pokyny k PNP PowerShellu, které popisují možnosti a [nástroje, které](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) můžete používat dnes k používání klasického režimu.</span><span class="sxs-lookup"><span data-stu-id="255d9-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
