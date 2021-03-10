---
title: Konfigurace a ověření vyloučení pro MDATP na počítači s Linuxem
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693344"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="070be-102">Konfigurace a ověření vyloučení pro MDATP na počítači s Linuxem</span><span class="sxs-lookup"><span data-stu-id="070be-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="070be-103">Z naskenovaných protokolu MDATP můžete vyloučit určité soubory, složky, procesy a soubory otevřené procesem.</span><span class="sxs-lookup"><span data-stu-id="070be-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="070be-104">Vyloučení pomáhají zabránit nesprávnému rozpoznávání softwaru a souborů jedinečných nebo přizpůsobených vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="070be-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="070be-105">Vyloučení také pomáhají zmírnit problémy s výkonem způsobené rozhraním MDATP.</span><span class="sxs-lookup"><span data-stu-id="070be-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="070be-106">Další informace najdete v článku Konfigurace a ověření vyloučení pro [MDATP pro Linux.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="070be-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="070be-107">Vyloučení popsaná v tomto článku se nevztahují na další funkce MDATP pro Linux, včetně zjišťování koncových bodů a odpovědí (EDR).</span><span class="sxs-lookup"><span data-stu-id="070be-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="070be-108">Soubory, které vyloučíte pomocí metod popsaných v tomto článku, mohou stále aktivovat upozornění EDR a další možnosti zjišťování.</span><span class="sxs-lookup"><span data-stu-id="070be-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
