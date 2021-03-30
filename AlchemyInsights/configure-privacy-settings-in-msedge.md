---
title: Konfigurace nastavení ochrany osobních údajů v Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404375"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="082c2-102">Konfigurace nastavení ochrany osobních údajů v Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="082c2-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="082c2-103">Pokud je Microsoft Edge nasazený na platformách mimo Windows, diagnostická data a informace o webu se ve výchozím nastavení microsoftu neposílanou.</span><span class="sxs-lookup"><span data-stu-id="082c2-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="082c2-104">Pokud je ale Microsoft Edge nasazený ve Windows 10, posílají se diagnostická data a informace o webu podle nastavení diagnostických dat [Windows uživatelů.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="082c2-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="082c2-105">Pokud chcete nakonfigurovat, jak Microsoft Edge zpracovává shromažďování dat pro vaši organizaci, použijte následující zásady skupiny:</span><span class="sxs-lookup"><span data-stu-id="082c2-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="082c2-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) zapne vykazování využití a dat souvisejících s chybou.</span><span class="sxs-lookup"><span data-stu-id="082c2-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="082c2-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) odesílá informace o webu, které se používají ke zlepšování služeb Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="082c2-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="082c2-108">Další informace najdete v tématu [Konfigurace nastavení zásad](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="082c2-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
