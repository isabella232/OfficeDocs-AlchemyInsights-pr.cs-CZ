---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770984"
---
# <a name="verify-your-domain"></a><span data-ttu-id="c5ae8-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="c5ae8-102">Verify your domain</span></span>

 <span data-ttu-id="c5ae8-103">**Záznam se pravděpodobně ne aktualizoval na internetu.**</span><span class="sxs-lookup"><span data-stu-id="c5ae8-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="c5ae8-104">Nový záznam zpravidla vidíme za několik minut, občas to ale může trvat i několik hodin.</span><span class="sxs-lookup"><span data-stu-id="c5ae8-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="c5ae8-105">Pokud už jste dlouho čekali, zkontrolujte, že jste zkopíroval(a) a vkopíroval(a) přesnou hodnotu do ověřovacího záznamu TXT u hostitele DNS.</span><span class="sxs-lookup"><span data-stu-id="c5ae8-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="c5ae8-106">Jedním z běžných problémů je, že součástí tohoto záznamu není text „MS=".</span><span class="sxs-lookup"><span data-stu-id="c5ae8-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="c5ae8-107">Je to ale nezbytné!</span><span class="sxs-lookup"><span data-stu-id="c5ae8-107">We need that too!</span></span>

- <span data-ttu-id="c5ae8-108">U některých hostitelů DNS musíte k uložení soubory zóny (kde je tento záznam DNS uložený) použít dodatečný krok, aby se aktualizoval v internetu.</span><span class="sxs-lookup"><span data-stu-id="c5ae8-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="c5ae8-109">Ujistěte se, že jste změny uložili, aby Microsoft mohl záznam zobrazit a ověřit.</span><span class="sxs-lookup"><span data-stu-id="c5ae8-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
