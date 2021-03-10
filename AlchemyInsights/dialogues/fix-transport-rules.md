---
title: Oprava pravidel přenosu
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693296"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="5abc5-102">Oprava pravidel přenosu</span><span class="sxs-lookup"><span data-stu-id="5abc5-102">Fix transport rules</span></span>

<span data-ttu-id="5abc5-103">Tuto zprávu ovlivnilo vlastní pravidlo toku pošty.</span><span class="sxs-lookup"><span data-stu-id="5abc5-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="5abc5-104">Když chcete zkontrolovat přesné pravidlo, proveďte toto:</span><span class="sxs-lookup"><span data-stu-id="5abc5-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="5abc5-105">Ve výsledcích odeslání si v části **Další informace** poznamenejte **identifikátor GUID** nebo **název zásady.**</span><span class="sxs-lookup"><span data-stu-id="5abc5-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="5abc5-106">Spusťte prostředí Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="5abc5-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="5abc5-107">Další informace najdete v článku [o otevření prostředí Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="5abc5-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="5abc5-108">Spusťte tento příkaz (pomocí identifikátoru GUID pro odeslání):  **Get-TransportRule -identity "GUID" | fl \* Popis**\*</span><span class="sxs-lookup"><span data-stu-id="5abc5-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="5abc5-109">Prohlédněte si popis a podívejte se na nakonfigurované podmínky, které zprávu ovlivnily.</span><span class="sxs-lookup"><span data-stu-id="5abc5-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="5abc5-110">Další informace najdete v [tématu Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="5abc5-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
