---
title: Odebrání dat a vymazání zařízení z Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439154"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odebrání dat a vymazání zařízení z Intune

Vzdálené akce Vyřazení zařízení a Vymazání zařízení lze použít k odebrání firemních dat spravovaných službou Intune nebo k obnovení továrního nastavení a vrácení zařízení do výchozího nastavení.

1. Přihlaste se ke správě zařízení Microsoft 365 a přejděte na **Zařízení**  >  **všechna zařízení**.
2. Vyberte zařízení, které chcete vymazat.
3. Vyberte typ vzdáleného vymazání, které chcete provést. Vyřazení odstraní pouze informace organizace, zatímco úplné vymazání obnoví zařízení do továrního nastavení.
4. Chcete-li potvrdit, vyberte **možnost Ano.** Dokud vymazání neskončí, stav akce Zařízení se zobrazí jako Vyřazení čeká na vyřízení.</br>
    Po dokončení akce se mobilní zařízení v seznamu spravovaného zařízení už nebude zobrazovat.

**Poznámka:** Firemní data nelze odebrat ze zařízení, která jsou připojena k Azure AD.

Podrobné informace o účincích akcí Vyřazení a vymazání, včetně toho, co je zachováno a co se odstraní, najdete [v tématu Odebrání zařízení pomocí vymazání, vyřazení nebo ručního zrušení registrace zařízení](https://docs.microsoft.com/intune/devices-wipe).

Pokud chcete vymazat všechna data ze zařízení s macOS, [přečtěte si přečtěte si přečtěte si tématu Vymazání všech dat ze zařízení s macOS.](https://docs.microsoft.com/intune/device-erase)