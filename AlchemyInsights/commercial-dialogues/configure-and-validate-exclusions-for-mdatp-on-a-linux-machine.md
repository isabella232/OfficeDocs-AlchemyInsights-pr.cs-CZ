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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744537"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="5bf9a-102">Konfigurace a ověření vyloučení pro MDATP na počítači s Linuxem</span><span class="sxs-lookup"><span data-stu-id="5bf9a-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="5bf9a-103">Některé soubory, složky, procesy a soubory otevřené procesem můžete z kontroly MDATP vyloučit.</span><span class="sxs-lookup"><span data-stu-id="5bf9a-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="5bf9a-104">Vyloučení pomáhají zabránit nesprávné detekci softwaru a souborů jedinečných nebo přizpůsobených vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="5bf9a-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="5bf9a-105">Vyloučení také pomáhají zmírnit problémy s výkonem způsobené MDATP.</span><span class="sxs-lookup"><span data-stu-id="5bf9a-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="5bf9a-106">Další informace najdete v tématu Konfigurace a [ověření vyloučení pro MDATP pro Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="5bf9a-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5bf9a-107">Vyloučení popsaná v tomto článku se nevztahují na jiné funkce MDATP pro Linux, včetně zjišťování koncových bodů a odpovědi (EDR).</span><span class="sxs-lookup"><span data-stu-id="5bf9a-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="5bf9a-108">Soubory, které vyloučíte pomocí metod popsaných v tomto článku, mohou pořád aktivovat upozornění EDR a další možnosti zjišťování.</span><span class="sxs-lookup"><span data-stu-id="5bf9a-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
