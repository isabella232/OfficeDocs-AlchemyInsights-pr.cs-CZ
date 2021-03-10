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
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Zařízení mimo Windows z Rozšířené ochrany před internetovou ochranou v programu Microsoft Defender (ATP)

Postup:

1. Podle dokumentace od jiného výrobce odpojte řešení třetí strany od poskytovatele ochrany před internetovou útoky v programu Microsoft Defender.
2. Z tenanta Azure Active Directory odeberte oprávnění pro řešení třetí strany:

    1. Přihlaste se k [portálu Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)
    1. Vyberte **všechny služby** Azure Active  >  **Directory** Enterprise  >  **Applications.**
    1. Vyberte aplikaci, kterou chcete vypnout.
    1. Vyberte **Odstranit.**

Další informace najdete v tématu [Offboard zařízení bez Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)
