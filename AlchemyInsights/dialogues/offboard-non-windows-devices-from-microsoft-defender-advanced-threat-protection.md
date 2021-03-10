---
title: Zařízení mimo Windows z Rozšířené ochrany před internetovou ochranou v programu Microsoft Defender (ATP)
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
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693095"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="c00dc-102">Zařízení mimo Windows z Rozšířené ochrany před internetovou ochranou v programu Microsoft Defender (ATP)</span><span class="sxs-lookup"><span data-stu-id="c00dc-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="c00dc-103">Postup:</span><span class="sxs-lookup"><span data-stu-id="c00dc-103">Here's how:</span></span>

1. <span data-ttu-id="c00dc-104">Podle dokumentace od jiného výrobce odpojte řešení třetí strany od poskytovatele ochrany před internetovou útoky v programu Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="c00dc-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="c00dc-105">Z tenanta Azure Active Directory odeberte oprávnění pro řešení třetí strany:</span><span class="sxs-lookup"><span data-stu-id="c00dc-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="c00dc-106">Přihlaste se k [portálu Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="c00dc-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="c00dc-107">Vyberte **všechny služby** Azure Active  >  **Directory** Enterprise  >  **Applications.**</span><span class="sxs-lookup"><span data-stu-id="c00dc-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="c00dc-108">Vyberte aplikaci, kterou chcete vypnout.</span><span class="sxs-lookup"><span data-stu-id="c00dc-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="c00dc-109">Vyberte **Odstranit.**</span><span class="sxs-lookup"><span data-stu-id="c00dc-109">Select **Delete**.</span></span>

<span data-ttu-id="c00dc-110">Další informace najdete v tématu [Offboard zařízení bez Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="c00dc-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
