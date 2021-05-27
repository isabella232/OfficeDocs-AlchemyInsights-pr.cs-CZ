---
title: Stav senzoru kontroly koncových bodů v programu Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676100"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="8d720-102">Stav senzoru kontroly koncových bodů v programu Defender</span><span class="sxs-lookup"><span data-stu-id="8d720-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="8d720-103">Dlaždice **Zařízení s problémy se** senzorem je umístěná na řídicím panelu Operace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="8d720-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="8d720-104">Tato dlaždice obsahuje informace o možnosti jednotlivých zařízení poskytovat data ze senzorů a komunikovat se službou Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="8d720-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="8d720-105">Uvádí, kolik zařízení vyžaduje pozornost, a pomáhá vám identifikovat problematická zařízení a přijmout opatření k opravě známých problémů.</span><span class="sxs-lookup"><span data-stu-id="8d720-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="8d720-106">Dva indikátory stavu na dlaždici poskytují informace o počtu zařízení, která se službě nehladí správně:</span><span class="sxs-lookup"><span data-stu-id="8d720-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="8d720-107">**Nesprávně nakonfigurované** Zařízení, která můžou částečně vykazovat data senzorů službě Defender for Endpoint a můžou mít chyby konfigurace, které je potřeba opravit.</span><span class="sxs-lookup"><span data-stu-id="8d720-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="8d720-108">**Neaktivní** Zařízení, která přestala vykazovat službu Defender for Endpoint za poslední měsíc déle než sedm dní.</span><span class="sxs-lookup"><span data-stu-id="8d720-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="8d720-109">Kliknutím na libovolnou skupinu vás přesměruje na seznam Zařízení, který je filtrovaný podle vašich možností.</span><span class="sxs-lookup"><span data-stu-id="8d720-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="8d720-110">V seznamu Zařízení můžete seznam stavu filtrovat podle následujícího stavu:</span><span class="sxs-lookup"><span data-stu-id="8d720-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="8d720-111">**Aktivní** Zařízení, která aktivně hlásí službě Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="8d720-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="8d720-112">**Nesprávně nakonfigurované** Zařízení, která můžou částečně vykazovat data senzorů službě Defender for Endpoint, ale mají chyby konfigurace, které je potřeba opravit.</span><span class="sxs-lookup"><span data-stu-id="8d720-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="8d720-113">Nesprávně nakonfigurovaná zařízení mohou mít jeden nebo kombinaci následujících problémů:</span><span class="sxs-lookup"><span data-stu-id="8d720-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="8d720-114">Žádná data ze senzoru – Zařízení přestala odesílat data ze senzoru.</span><span class="sxs-lookup"><span data-stu-id="8d720-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="8d720-115">Ze zařízení se pouštějí omezená upozornění.</span><span class="sxs-lookup"><span data-stu-id="8d720-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="8d720-116">Zhoršená komunikace – schopnost komunikovat se zařízením je zhoršená.</span><span class="sxs-lookup"><span data-stu-id="8d720-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="8d720-117">Odesílání souborů pro hloubkovou analýzu, blokování souborů, izolování zařízení ze sítě a další akce, které vyžadují komunikaci se zařízením, nemusí fungovat.</span><span class="sxs-lookup"><span data-stu-id="8d720-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="8d720-118">**Neaktivní** Zařízení, která přestala vykazovat zprávy službě Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="8d720-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="8d720-119">Pomocí funkce Exportovat si můžete stáhnout celý seznam ve formátu CSV.</span><span class="sxs-lookup"><span data-stu-id="8d720-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="8d720-120">Další informace najdete v tématu [Kontrola stavu senzoru v programu Microsoft Defender pro koncový bod](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="8d720-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="8d720-121">Další informace o tom, co způsobilo, že zařízení bylo neaktivní nebo nesprávně nakonfigurované, najdete v článku Oprava chybných [senzorů](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)v Programu Microsoft Defender pro koncový bod .</span><span class="sxs-lookup"><span data-stu-id="8d720-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
