---
title: Nástroj pro diagnostiku služby pro virtuální plochu Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595517"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="486b0-102">Nástroj pro diagnostiku služby pro virtuální plochu Windows</span><span class="sxs-lookup"><span data-stu-id="486b0-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="486b0-103">Windows Virtual Desktop (WVD) nabízí diagnostický nástroj, který správcům umožňuje identifikovat chyby prostřednictvím jednoho rozhraní.</span><span class="sxs-lookup"><span data-stu-id="486b0-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="486b0-104">Tento nástroj zaznamenává informace související s diagnostikou při každém použití funkce WVD někým, kdo má přiřazenou roli WVD.</span><span class="sxs-lookup"><span data-stu-id="486b0-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="486b0-105">Každý protokol obsahuje informace o roli WVD, která je součástí aktivity, chybové zprávy, které se zobrazují během relace, a informace o tenantovi a uživateli.</span><span class="sxs-lookup"><span data-stu-id="486b0-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="486b0-106">Azure Log Analytics můžete nakonfigurovat tak, aby zachycoval protokol aktivit vytvořený diagnostickým nástrojem takto:</span><span class="sxs-lookup"><span data-stu-id="486b0-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="486b0-107">Vytvořte pracovní prostor Log Analytics pomocí [portálu Azure portal nebo](https://go.microsoft.com/fwlink/?linkid=2129500) Azure [PowerShellu.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="486b0-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="486b0-108">[Připojte počítače s Windows k Azure Monitoru.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="486b0-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="486b0-109">Získejte ID pracovního prostoru a primární klíč pracovního prostoru.</span><span class="sxs-lookup"><span data-stu-id="486b0-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="486b0-110">Průvodce nastavením potřebuje tyto informace, aby mohl správně nakonfigurovat agenta a zajistit, aby mohl komunikovat s Azure Monitorem.</span><span class="sxs-lookup"><span data-stu-id="486b0-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="486b0-111">[Předáte diagnostická data do pracovního prostoru.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="486b0-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="486b0-112">Diagnostická data z tenanta WVD můžete předát do analýzy protokolů pro váš pracovní prostor.</span><span class="sxs-lookup"><span data-stu-id="486b0-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="486b0-113">[Identifikujte a diagnostikujte](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problémy, které jsou ve vztahu k WVD interní nebo externí.</span><span class="sxs-lookup"><span data-stu-id="486b0-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="486b0-114">Další informace o konfiguraci nástroje pro diagnostiku služby pro službu WVD najdete v tématu Použití analýzy protokolů pro funkci diagnostiky.</span><span class="sxs-lookup"><span data-stu-id="486b0-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>