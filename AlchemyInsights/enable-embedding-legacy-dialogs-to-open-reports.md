---
title: Povolení vkládání zastaralých dialogů pro otevření sestav
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814257"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="87c28-102">Povolení vkládání zastaralých dialogů pro otevření sestav</span><span class="sxs-lookup"><span data-stu-id="87c28-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="87c28-103">**Příznak**</span><span class="sxs-lookup"><span data-stu-id="87c28-103">**Symptom**</span></span>

<span data-ttu-id="87c28-104">Uživatelům se nedaří otevřít sestavy.</span><span class="sxs-lookup"><span data-stu-id="87c28-104">Users are unable to open reports.</span></span> <span data-ttu-id="87c28-105">„Došlo k nějakému problému.</span><span class="sxs-lookup"><span data-stu-id="87c28-105">"Something has gone wrong.</span></span> <span data-ttu-id="87c28-106">Další informace najdete v technických podrobnostech.“</span><span class="sxs-lookup"><span data-stu-id="87c28-106">Check technical details for more details."</span></span>

<span data-ttu-id="87c28-107">**Příčina**</span><span class="sxs-lookup"><span data-stu-id="87c28-107">**Cause**</span></span>

<span data-ttu-id="87c28-108">Sestavy se nedaří načíst do nástroje UCI a zobrazuje se chybová zpráva: „Popisovač formuláře je null nebo není definovaný.“</span><span class="sxs-lookup"><span data-stu-id="87c28-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="87c28-109">Sestavy v nástroji UCI vyžadují starší verze dialogů, takže systém zákazníka musí mít povolenou funkci *allowlegacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="87c28-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="87c28-110">**Řešení**</span><span class="sxs-lookup"><span data-stu-id="87c28-110">**Solution**</span></span>

1. <span data-ttu-id="87c28-111">Přejděte na **Nastavení > Správa > Nastavení systému > karta Obecné**.</span><span class="sxs-lookup"><span data-stu-id="87c28-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="87c28-112">Nastavte možnost „Povolí vkládání určitých zastaralých dialogů do klienta prohlížeče Sjednoceného rozhraní“ na **Ano**.</span><span class="sxs-lookup"><span data-stu-id="87c28-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
