---
title: Problémy s odebráním offboarded nebo vyřazené zařízení z inventáře zařízení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564078"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="2f65c-102">Problémy s odebráním offboarded nebo vyřazené zařízení z inventáře zařízení</span><span class="sxs-lookup"><span data-stu-id="2f65c-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="2f65c-103">Microsoft Defender pro koncový bod v současné době neumožňuje ručně odebrat záznam zařízení z inventáře zařízení, které je vypnuté nebo vyřazené z provozu.</span><span class="sxs-lookup"><span data-stu-id="2f65c-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="2f65c-104">Z bezpečnostních důvodů zůstane zařízení na portálu jako historický záznam po dobu až 180 dnů.</span><span class="sxs-lookup"><span data-stu-id="2f65c-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="2f65c-105">Data zařízení se ale vyprázdní podle nakonfigurované doby uchovávání.</span><span class="sxs-lookup"><span data-stu-id="2f65c-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="2f65c-106">**Poznámka:** Vypnuté nebo vyřazené zařízení se  po sedmi dnech automaticky přepne do neaktivního stavu.</span><span class="sxs-lookup"><span data-stu-id="2f65c-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="2f65c-107">Kromě toho se zařízení, která nejsou aktivní v posledních 30 dnech, nevedou do dat, která odrážejí skóre expozice vaší organizace Threat and Vulnerability Management nebo Microsoft Secure Score for Devices.</span><span class="sxs-lookup"><span data-stu-id="2f65c-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="2f65c-108">Pokud nechcete některá zařízení v zobrazení Inventář zařízení zobrazit, zkuste umístit značku zařízení a vyfiltrovat vyřazené zařízení ze zobrazení Inventář zařízení.</span><span class="sxs-lookup"><span data-stu-id="2f65c-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="2f65c-109">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="2f65c-109">For more information, see:</span></span>

[<span data-ttu-id="2f65c-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="2f65c-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="2f65c-111">Skóre expozice v Threat and Vulnerability Management</span><span class="sxs-lookup"><span data-stu-id="2f65c-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="2f65c-112">Oprava nefunkčových senzorů v Microsoft Defenderu pro koncový bod</span><span class="sxs-lookup"><span data-stu-id="2f65c-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="2f65c-113">Jak efektivně používat označování (část 1)</span><span class="sxs-lookup"><span data-stu-id="2f65c-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="2f65c-114">Jak efektivně používat označování (část 2)</span><span class="sxs-lookup"><span data-stu-id="2f65c-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="2f65c-115">Jak efektivně používat označování (část 3)</span><span class="sxs-lookup"><span data-stu-id="2f65c-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




