---
title: Graf znázorňuje různý počet záznamů v tabulce.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793751"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="d5777-102">Graf znázorňuje různý počet záznamů v tabulce.</span><span class="sxs-lookup"><span data-stu-id="d5777-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="d5777-103">**Příznak**</span><span class="sxs-lookup"><span data-stu-id="d5777-103">**Symptom**</span></span>

<span data-ttu-id="d5777-104">Na stránce graf na řídicím panelu, když kliknete na graf "..." a kliknutím na možnost zobrazit záznamy přejdete na stránku mřížka, kde zobrazíte všechny záznamy. Někdy se počet záznamů změní.</span><span class="sxs-lookup"><span data-stu-id="d5777-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="d5777-105">Tato část obsahuje přehledné informace o problému a osobě, která ho má odstranit. Na obrázku vidíte tři základní strany v transakci e-mailu Office 365 - odesílatele, Office 365 a příjemce. Červeně označená oblast je oblast, ve které je obvykle potřeba problém odstranit.</span><span class="sxs-lookup"><span data-stu-id="d5777-105">**Cause**</span></span>

<span data-ttu-id="d5777-106">Důvodem je rozdíl mezi zobrazeními mezi grafem na původní stránce řídicího panelu a grafem na domovské stránce mřížky.</span><span class="sxs-lookup"><span data-stu-id="d5777-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="d5777-107">**Řešení**</span><span class="sxs-lookup"><span data-stu-id="d5777-107">**Solution**</span></span>

1. <span data-ttu-id="d5777-108">Zkontrolujte zobrazení z původní stránky a zobrazení v mřížce, jestli se liší.</span><span class="sxs-lookup"><span data-stu-id="d5777-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="d5777-109">Změňte zobrazení v mřížce tak, aby odpovídalo zobrazení na původní stránce.</span><span class="sxs-lookup"><span data-stu-id="d5777-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="d5777-110">Pokud nejde najít správné zobrazení, obvykle to znamená, že zobrazení není v Návrháři aplikací povolené.</span><span class="sxs-lookup"><span data-stu-id="d5777-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="d5777-111">Přejděte na Návrhář aplikací určité aplikace, zvolte entitu a její zobrazení, zaškrtněte zobrazení, které chcete povolit, uložit, publikovat a zavřít.</span><span class="sxs-lookup"><span data-stu-id="d5777-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="d5777-112">Aktualizujte stránku.</span><span class="sxs-lookup"><span data-stu-id="d5777-112">Refresh the page.</span></span>