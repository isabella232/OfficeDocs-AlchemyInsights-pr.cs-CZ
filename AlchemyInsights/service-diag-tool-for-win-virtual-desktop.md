---
title: Nástroj pro diagnostiku služeb pro virtuální plochu Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677652"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="fbdb8-102">Nástroj pro diagnostiku služeb pro virtuální plochu Windows</span><span class="sxs-lookup"><span data-stu-id="fbdb8-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="fbdb8-103">Virtual Desktop (WVD) systému Windows nabízí diagnostický nástroj, který správcům umožňuje identifikovat chyby prostřednictvím jednoho rozhraní.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="fbdb8-104">Tento nástroj slouží k protokolování informací o diagnostice, kdykoli WVD používá někdo přiřazený roli WVD.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="fbdb8-105">Každý protokol obsahuje informace o roli WVD zahrnuté v aktivitě, chybové zprávy, které se zobrazí během relace, a informace o tenantovi a uživateli.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="fbdb8-106">Analýzu protokolů Azure je možné nakonfigurovat tak, aby zachytával protokol aktivit vytvořený diagnostickým nástrojem.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="fbdb8-107">Postup:</span><span class="sxs-lookup"><span data-stu-id="fbdb8-107">Here's how:</span></span>

1. <span data-ttu-id="fbdb8-108">Vytvořte pracovní prostor analýzy protokolů pomocí [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) nebo [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="fbdb8-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="fbdb8-109">[Připojte počítače se systémem Windows ke službě Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="fbdb8-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="fbdb8-110">Získejte ID pracovního prostoru a primární klíč pracovního prostoru.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="fbdb8-111">Průvodce instalací potřebuje tyto informace, aby správně nakonfiguroval agenta a zajistil komunikaci s Azure monitorem.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="fbdb8-112">[Zatlačte data diagnostiky do pracovního prostoru](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="fbdb8-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="fbdb8-113">Data diagnostiky můžete zatlačit z tenanta WVD do analýzy protokolů pro váš pracovní prostor.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="fbdb8-114">[Identifikujte a Diagnostikujte problémy](https://go.microsoft.com/fwlink/?linkid=2128338) , které jsou ve vztahu k WVD vnitřní nebo externí.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="fbdb8-115">Další informace o konfiguraci nástroje pro diagnostiku služeb pro WVD najdete v tématu [použití funkce Analýza protokolů pro funkci diagnostiky](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="fbdb8-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
