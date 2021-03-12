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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744669"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="e464c-102">Automatické přesouvání zpráv do archivu</span><span class="sxs-lookup"><span data-stu-id="e464c-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="e464c-103">Pokud používáte zásady uchovávání informací, můžete změnit věk uchovávání informací v této zásadách tak, aby se zprávy automaticky archivovány přestaly archivovat.</span><span class="sxs-lookup"><span data-stu-id="e464c-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="e464c-104">Postup:</span><span class="sxs-lookup"><span data-stu-id="e464c-104">Here's how:</span></span>

1. <span data-ttu-id="e464c-105">V Centru [pro správu Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)zvolte značky uchovávání informací pro **správu**  >  **dodržování předpisů**.</span><span class="sxs-lookup"><span data-stu-id="e464c-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="e464c-106">Vyhledejte značku uchovávání informací přesunout do archivu.</span><span class="sxs-lookup"><span data-stu-id="e464c-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="e464c-107">Ve značce uchovávání informací změňte dobu  uchovávání informací (archivační období) na Nikdy, aby se položky automaticky archivoval pomocí zásad uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="e464c-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="e464c-108">Tím se změní nastavení archivu pro všechny poštovní schránky s touto značkou uchovávání informací, která se na ně použije.</span><span class="sxs-lookup"><span data-stu-id="e464c-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
