---
title: MC210173 – vyřazení nové vlastní funkce formulářů v SharePoint Designeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831799"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="319af-102">MC210173 – vyřazení nové vlastní funkce formulářů v SharePoint Designeru</span><span class="sxs-lookup"><span data-stu-id="319af-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="319af-103">Zjistili jsme problém ovlivňující funkce SharePoint Designeru pro [vytváření vlastních formulářů](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) v SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="319af-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="319af-104">Po pečlivém přezkoumání jsme zjistili, že pro tento problém není k dispozici žádná známá oprava tohoto problému, a rozhodli jsme se s platností od 3:00 soboty 25. dubna 2020 funkci vytváření vlastních formulářů zablokovat.</span><span class="sxs-lookup"><span data-stu-id="319af-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="319af-105">Tato změna neovlivní možnost upravovat dříve vytvořené formuláře nebo jiné existující funkce v návrháři SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="319af-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="319af-106">Po provedení této změny se může stát, že se uživatelům při vytváření nových formulářů zobrazí chyba typu Nejde uložit změny seznamu na server.</span><span class="sxs-lookup"><span data-stu-id="319af-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="319af-107">Uživatelé, kteří dřív k vytváření vlastních formulářů využívali SharePoint Designer, teď mohou k tomuto účelu použít [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="319af-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="319af-108">PowerApps je jednoduchý a výkonný nástroj, který umožňuje uživatelům pracujícím v moderním prostředí SharePointu Online vytvářet a upravovat vlastní formuláře pro seznamy a knihovny dokumentů SharePointu přímo z okna prohlížeče.</span><span class="sxs-lookup"><span data-stu-id="319af-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="319af-109">PowerApps nevyžaduje tradiční znalosti kódování ani žádné stahování dalších aplikací, jako je třeba InfoPath.</span><span class="sxs-lookup"><span data-stu-id="319af-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="319af-110">**Poznámka:** Uživatelé SharePointu Online v klasickém režimu budou muset dočasně přepnout na moderní prostředí, aby měli přístup k PowerApps a mohli tuto aplikaci využívat. Všechny vlastní formuláře vytvořené v PowerApps jsou ale pro uživatele klasického režimu SharePointu Online přístupné.</span><span class="sxs-lookup"><span data-stu-id="319af-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
