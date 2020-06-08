---
title: Povolení vkládání starších dialogových oken k otevření sestav
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204653"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="ff3ad-102">Povolení vkládání starších dialogových oken k otevření sestav</span><span class="sxs-lookup"><span data-stu-id="ff3ad-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="ff3ad-103">**Příznakem**</span><span class="sxs-lookup"><span data-stu-id="ff3ad-103">**Symptom**</span></span>

<span data-ttu-id="ff3ad-104">Uživatelé nemohou otevřít sestavy.</span><span class="sxs-lookup"><span data-stu-id="ff3ad-104">Users are unable to open reports.</span></span> <span data-ttu-id="ff3ad-105">"Něco se pokazilo.</span><span class="sxs-lookup"><span data-stu-id="ff3ad-105">"Something has gone wrong.</span></span> <span data-ttu-id="ff3ad-106">Další podrobnosti naleznete v technických podrobnostech."</span><span class="sxs-lookup"><span data-stu-id="ff3ad-106">Check technical details for more details."</span></span>

<span data-ttu-id="ff3ad-107">Tato část obsahuje přehledné informace o problému a osobě, která ho má odstranit. Na obrázku vidíte tři základní strany v transakci e-mailu Office 365 - odesílatele, Office 365 a příjemce. Červeně označená oblast je oblast, ve které je obvykle potřeba problém odstranit.</span><span class="sxs-lookup"><span data-stu-id="ff3ad-107">**Cause**</span></span>

<span data-ttu-id="ff3ad-108">Sestavy se nedaří načíst v UCI s chybou "Popisovač formuláře je null nebo není definován."</span><span class="sxs-lookup"><span data-stu-id="ff3ad-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="ff3ad-109">Sestavy v UCI stále vyžadují starší dialogová okna, takže systém zákazníka musí mít *povoleno povolené delegacydialogsemdding.*</span><span class="sxs-lookup"><span data-stu-id="ff3ad-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="ff3ad-110">**Řešení**</span><span class="sxs-lookup"><span data-stu-id="ff3ad-110">**Solution**</span></span>

1. <span data-ttu-id="ff3ad-111">Přejděte na **kartu Nastavení >správa > nastavení systému > obecné**.</span><span class="sxs-lookup"><span data-stu-id="ff3ad-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="ff3ad-112">Možnost Povolit vkládání určitých starších dialogových oken v klientovi prohlížeče sjednoceného rozhraní na **možnost Ano**.</span><span class="sxs-lookup"><span data-stu-id="ff3ad-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
