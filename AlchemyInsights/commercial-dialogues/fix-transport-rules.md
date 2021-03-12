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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744843"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="8c9bb-102">Oprava pravidel přenosu</span><span class="sxs-lookup"><span data-stu-id="8c9bb-102">Fix transport rules</span></span>

<span data-ttu-id="8c9bb-103">Tato zpráva se týká vlastního pravidla toku pošty.</span><span class="sxs-lookup"><span data-stu-id="8c9bb-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="8c9bb-104">Pokud chcete zkontrolovat přesné pravidlo, proveďte toto:</span><span class="sxs-lookup"><span data-stu-id="8c9bb-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="8c9bb-105">Ve výsledcích odeslání si v části **Další informace** poznamenejte **identifikátor GUID** nebo název **zásady**.</span><span class="sxs-lookup"><span data-stu-id="8c9bb-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="8c9bb-106">Spusťte Prostředí Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="8c9bb-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="8c9bb-107">Další informace najdete v tématu [Otevření prostředí Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="8c9bb-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="8c9bb-108">Spusťte tento příkaz (pomocí identifikátoru GUID z odeslání):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="8c9bb-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="8c9bb-109">V popisu se zobrazí nakonfigurované podmínky, které ovlivnily zprávu.</span><span class="sxs-lookup"><span data-stu-id="8c9bb-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="8c9bb-110">Další informace najdete v tématu [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="8c9bb-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
