---
title: Zakázat kontrolu sítě
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481126"
---
# <a name="disable-network-scan"></a><span data-ttu-id="9abff-102">Zakázat kontrolu sítě</span><span class="sxs-lookup"><span data-stu-id="9abff-102">Disable network scan</span></span>

<span data-ttu-id="9abff-103">Může to mít vliv na skenování sdílené síťové složky.</span><span class="sxs-lookup"><span data-stu-id="9abff-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="9abff-104">Pokud chcete zajistit, aby klient ve výchozím nastavení neprohledl sdílené síťové složky nebo soubory, nakonfigurujte v aplikaci Windows Defender následující nastavení na **Pravdivé:**</span><span class="sxs-lookup"><span data-stu-id="9abff-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="9abff-105">DisableScanningMappedNetworkDrivesForFullNetwork</span><span class="sxs-lookup"><span data-stu-id="9abff-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="9abff-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="9abff-106">DisableScanningNetworkFiles</span></span>