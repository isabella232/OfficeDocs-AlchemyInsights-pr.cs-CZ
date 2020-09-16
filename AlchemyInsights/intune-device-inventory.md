---
title: Intune – inventář zařízení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667871"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="0c83d-102">Intune – inventář zařízení</span><span class="sxs-lookup"><span data-stu-id="0c83d-102">Intune Device Inventory</span></span>

<span data-ttu-id="0c83d-103">Okno zařízení poskytuje správci přehled o zařízeních ve správě v Intune na jednotlivých zařízeních.</span><span class="sxs-lookup"><span data-stu-id="0c83d-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="0c83d-104">Zobrazené informace zahrnují: hardware, zjištěné aplikace, stav shody zařízení a stav konfigurace zařízení.</span><span class="sxs-lookup"><span data-stu-id="0c83d-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="0c83d-105">Data inventáře pro hardware a zjištěné aplikace se shromažďují po sedmi dnech.</span><span class="sxs-lookup"><span data-stu-id="0c83d-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="0c83d-106">Uvedené aplikace a zvláštní prvky hardwaru se liší v závislosti na operačním systému zařízení a na tom, jestli je dané zařízení osobně nebo podnikově vlastněné.</span><span class="sxs-lookup"><span data-stu-id="0c83d-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="0c83d-107">Další informace najdete v tématu [zobrazení podrobností o zařízení v Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="0c83d-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="0c83d-108">**Nejčastější dotazy**</span><span class="sxs-lookup"><span data-stu-id="0c83d-108">**FAQ**</span></span>

<span data-ttu-id="0c83d-109">Otázka: mi se nezobrazuje seznam úplný soupis aplikací v Intune – registrovaná zařízení s Windows.</span><span class="sxs-lookup"><span data-stu-id="0c83d-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="0c83d-110">Proč ne?</span><span class="sxs-lookup"><span data-stu-id="0c83d-110">Why not?</span></span>

<span data-ttu-id="0c83d-111">A: pro počítače s Windows 10, které jsou označené jako podniková zařízení, jsou v současnosti uvedené jenom moderní aplikace.</span><span class="sxs-lookup"><span data-stu-id="0c83d-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="0c83d-112">Intune neshromažďuje informace o aplikacích Win32 nainstalovaných na těchto zařízeních.</span><span class="sxs-lookup"><span data-stu-id="0c83d-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="0c83d-113">Otázka: Proč se telefonní čísla neshromažďují ze všech zařízení?</span><span class="sxs-lookup"><span data-stu-id="0c83d-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="0c83d-114">A: telefony, které jsou v Intune zařazené do kategorií, se neidentifikují s plným telefonním číslem, když třeba spustíte sestavu inventáře mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="0c83d-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="0c83d-115">Osobní telefonní čísla zařízení jsou vždy částečně maskována pomocí hvězdiček (\* \* \* \*) a zobrazují jenom poslední čtyři číslice.</span><span class="sxs-lookup"><span data-stu-id="0c83d-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>