---
title: Inventář zařízení Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439161"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="e90bd-102">Inventář zařízení Intune</span><span class="sxs-lookup"><span data-stu-id="e90bd-102">Intune Device Inventory</span></span>

<span data-ttu-id="e90bd-103">Okno Zařízení poskytuje správci přehled o zařízeních, která jsou v rámci správy v Intune, a to na základě pro všechna zařízení.</span><span class="sxs-lookup"><span data-stu-id="e90bd-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="e90bd-104">Zobrazené informace zahrnují: Hardware, Zjištěné aplikace, Stav kompatibility zařízení a stav konfigurace zařízení.</span><span class="sxs-lookup"><span data-stu-id="e90bd-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="e90bd-105">Data inventáře pro hardware a zjištěné aplikace jsou shromažďována v sedmidenním cyklu.</span><span class="sxs-lookup"><span data-stu-id="e90bd-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="e90bd-106">Aplikace a konkrétní prvky hardwaru hlášené se liší v závislosti na operačním systému zařízení a zda je zařízení v osobním nebo vlastněném podniku.</span><span class="sxs-lookup"><span data-stu-id="e90bd-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="e90bd-107">Další informace najdete [v tématu Podrobnosti o zařízení v Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="e90bd-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="e90bd-108">**Nejčastější dotazy**</span><span class="sxs-lookup"><span data-stu-id="e90bd-108">**FAQ**</span></span>

<span data-ttu-id="e90bd-109">Otázka: Nedostávám úplný soupis aplikací, které se na zařízeních s Windows zaregistrované v Intune nacházejí.</span><span class="sxs-lookup"><span data-stu-id="e90bd-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="e90bd-110">Proč ne?</span><span class="sxs-lookup"><span data-stu-id="e90bd-110">Why not?</span></span>

<span data-ttu-id="e90bd-111">A: V současné době jsou uvedeny pouze moderní aplikace pro počítače s Windows 10, které jsou označeny jako podniková zařízení.</span><span class="sxs-lookup"><span data-stu-id="e90bd-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="e90bd-112">Intune neshromažďuje informace o aplikacích Win32 nainstalovaných na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="e90bd-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="e90bd-113">Otázka: Proč nejsou telefonní čísla shromažďována ze všech zařízení?</span><span class="sxs-lookup"><span data-stu-id="e90bd-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="e90bd-114">A: Telefony zařazené do kategorie podnikových zařízení v Intune nejsou identifikovány s jejich úplným telefonním číslem, když například spustíte přehled inventáře mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="e90bd-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="e90bd-115">Telefonní čísla bring-you-own-device jsou vždy částečně maskována hvězdičkami (\*\*\*\*) a zobrazují pouze poslední čtyři číslice.</span><span class="sxs-lookup"><span data-stu-id="e90bd-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>