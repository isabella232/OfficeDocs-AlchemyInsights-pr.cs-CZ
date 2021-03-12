---
title: Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744325"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="e5768-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="e5768-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="e5768-103">Postup:</span><span class="sxs-lookup"><span data-stu-id="e5768-103">Here's how:</span></span>

1. <span data-ttu-id="e5768-104">Podle dokumentace třetích stran odpojte řešení třetích stran od programu Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="e5768-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="e5768-105">Z tenanta Azure Active Directory odeberte oprávnění pro řešení třetích stran:</span><span class="sxs-lookup"><span data-stu-id="e5768-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="e5768-106">Přihlaste se k [portálu Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="e5768-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="e5768-107">Vyberte **Všechny služby** Azure Active  >  **Directory** Enterprise  >  **Applications**.</span><span class="sxs-lookup"><span data-stu-id="e5768-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="e5768-108">Vyberte aplikaci, kterou chcete vypnout.</span><span class="sxs-lookup"><span data-stu-id="e5768-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="e5768-109">Vyberte **Odstranit**.</span><span class="sxs-lookup"><span data-stu-id="e5768-109">Select **Delete**.</span></span>

<span data-ttu-id="e5768-110">Další informace najdete v tématu [Offboard zařízení, která nejsou zařízení s Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="e5768-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
