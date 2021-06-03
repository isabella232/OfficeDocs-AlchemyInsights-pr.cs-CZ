---
title: Microsoft Defender pro koncový bod v Linuxu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731342"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="33b39-102">Microsoft Defender pro koncový bod v Linuxu</span><span class="sxs-lookup"><span data-stu-id="33b39-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="33b39-103">Podrobnou dokumentaci k Linuxu najdete v [tématu Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span><span class="sxs-lookup"><span data-stu-id="33b39-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="33b39-104">Informace o systému a instalaci najdete v těchto článku:</span><span class="sxs-lookup"><span data-stu-id="33b39-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="33b39-105">Požadavky</span><span class="sxs-lookup"><span data-stu-id="33b39-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="33b39-106">Požadavky systému</span><span class="sxs-lookup"><span data-stu-id="33b39-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="33b39-107">Pokyny k instalaci</span><span class="sxs-lookup"><span data-stu-id="33b39-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="33b39-108">Síťová připojení</span><span class="sxs-lookup"><span data-stu-id="33b39-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="33b39-109">Pokyny najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="33b39-109">For instructions, see:</span></span>

- [<span data-ttu-id="33b39-110">Konfigurace nastavení proxy serveru zařízení a připojení k internetu</span><span class="sxs-lookup"><span data-stu-id="33b39-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="33b39-111">Nasazení aktualizací pro Microsoft Defender pro koncový bod v Linuxu</span><span class="sxs-lookup"><span data-stu-id="33b39-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="33b39-112">Jak nakonfigurovat Microsoft Defender pro koncový bod v Linuxu</span><span class="sxs-lookup"><span data-stu-id="33b39-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="33b39-113">Podporované příkazy</span><span class="sxs-lookup"><span data-stu-id="33b39-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="33b39-114">Potřebuji pomoct!</span><span class="sxs-lookup"><span data-stu-id="33b39-114">I need help!</span></span>

<span data-ttu-id="33b39-115">Pokud nemůžete najít informace nebo nápovědu, kterou hledáte, upřesníte hledaný řetězec.</span><span class="sxs-lookup"><span data-stu-id="33b39-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="33b39-116">Než se obraťte na podporu Microsoftu, nezapomeňte shromáždit data potřebná k prošetření vašeho problému a připojit je k lístku.</span><span class="sxs-lookup"><span data-stu-id="33b39-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="33b39-117">Postup shromažďování informací o diagnostice najdete v tématu [Shromažďování diagnostických dat](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span><span class="sxs-lookup"><span data-stu-id="33b39-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>