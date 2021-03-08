---
title: Automatické přesouvání zpráv do archivu
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524100"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="3741d-102">Automatické zastavení přesouvání zpráv do archivu</span><span class="sxs-lookup"><span data-stu-id="3741d-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="3741d-103">Pokud používáte zásady uchovávání informací, můžete v této zásadu změnit věk uchovávání informací a zabránit tak automatické archivaci zpráv.</span><span class="sxs-lookup"><span data-stu-id="3741d-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="3741d-104">Postup:</span><span class="sxs-lookup"><span data-stu-id="3741d-104">Here's how:</span></span>

1. <span data-ttu-id="3741d-105">V Centru [pro správu Exchange zvolte](https://go.microsoft.com/fwlink/?linkid=2059104)značky uchovávání informací **správy** dodržování  >  **předpisů.**</span><span class="sxs-lookup"><span data-stu-id="3741d-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="3741d-106">Vyhledejte značku uchovávání informací pro přesunutí do archivu.</span><span class="sxs-lookup"><span data-stu-id="3741d-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="3741d-107">Ve značce uchovávání informací změňte dobu  uchovávání informací (dobu archivace) tak, aby se nikdy nezastavoval automatický archiv položek pomocí zásad uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="3741d-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="3741d-108">Tím se změní nastavení archivace pro všechny poštovní schránky, u které je použita tato značka uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="3741d-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
