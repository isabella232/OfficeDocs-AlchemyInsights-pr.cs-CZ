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
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)

Postup:

1. Podle dokumentace třetích stran odpojte řešení třetích stran od programu Microsoft Defender ATP.
2. Z tenanta Azure Active Directory odeberte oprávnění pro řešení třetích stran:

    1. Přihlaste se k [portálu Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)
    1. Vyberte **Všechny služby** Azure Active  >  **Directory** Enterprise  >  **Applications**.
    1. Vyberte aplikaci, kterou chcete vypnout.
    1. Vyberte **Odstranit**.

Další informace najdete v tématu [Offboard zařízení, která nejsou zařízení s Windows](https://go.microsoft.com/fwlink/?linkid=2143630).
