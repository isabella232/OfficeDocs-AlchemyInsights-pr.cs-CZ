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
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – vyřazení nové vlastní funkce formulářů v SharePoint Designeru

Zjistili jsme problém ovlivňující funkce SharePoint Designeru pro [vytváření vlastních formulářů](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) v SharePointu Online. Po pečlivém přezkoumání jsme zjistili, že pro tento problém není k dispozici žádná známá oprava tohoto problému, a rozhodli jsme se s platností od 3:00 soboty 25. dubna 2020 funkci vytváření vlastních formulářů zablokovat. Tato změna neovlivní možnost upravovat dříve vytvořené formuláře nebo jiné existující funkce v návrháři SharePointu Online.

Po provedení této změny se může stát, že se uživatelům při vytváření nových formulářů zobrazí chyba typu Nejde uložit změny seznamu na server.

Uživatelé, kteří dřív k vytváření vlastních formulářů využívali SharePoint Designer, teď mohou k tomuto účelu použít [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

PowerApps je jednoduchý a výkonný nástroj, který umožňuje uživatelům pracujícím v moderním prostředí SharePointu Online vytvářet a upravovat vlastní formuláře pro seznamy a knihovny dokumentů SharePointu přímo z okna prohlížeče. PowerApps nevyžaduje tradiční znalosti kódování ani žádné stahování dalších aplikací, jako je třeba InfoPath.

**Poznámka:** Uživatelé SharePointu Online v klasickém režimu budou muset dočasně přepnout na moderní prostředí, aby měli přístup k PowerApps a mohli tuto aplikaci využívat. Všechny vlastní formuláře vytvořené v PowerApps jsou ale pro uživatele klasického režimu SharePointu Online přístupné.
