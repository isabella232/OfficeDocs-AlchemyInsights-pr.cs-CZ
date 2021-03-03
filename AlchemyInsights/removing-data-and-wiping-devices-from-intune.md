---
title: Odebrání dat a utírání zařízení z Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416306"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odebrání dat a utírání zařízení z Intune

Pomocí vzdálených akcí Vyřazení zařízení a Vymazání zařízení můžete odebrat data společnosti spravovaných Intune nebo obnovit tovární nastavení a vrátit zařízení do výchozího nastavení.

1. Přihlaste se ke Správě zařízení Microsoft 365 a přejděte na **Zařízení**  >  **všechna zařízení.**
2. Vyberte zařízení, které chcete vymazat.
3. Vyberte typ vzdáleného vymazání, které chcete udělat. Vyřazení odstraní jenom informace organizace, zatímco úplné vymazání obnoví zařízení do továrního nastavení.
4. Výběrem **možnosti Ano** potvrďte. Dokud se vymazání nedokončí, zobrazí se stav akce Zařízení jako Čeká na *vyřazení.*
    Po dokončení akce se už mobilní zařízení v seznamu spravovaného zařízení nebude zobrazit.

> [!NOTE]
> Ze zařízení PŘIPOJENÝch k Azure AD nelze odebrat data společnosti. 

Úplné podrobnosti o efektu akcí Vyřazení a vymazání, včetně toho, co se zachová a co se odstraní, najdete v následující dokumentaci:

- [Zařízení odeberte vymazáním, vyřazením nebo](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)ručním zrušení registrace zařízení.
- [Jak vymazat jenom podniková data z aplikací spravovaných přes Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Vymažte všechna data ze zařízení s macOS.](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)