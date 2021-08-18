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
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331034"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odebrání dat a utírání zařízení z Intune

Vzdálené akce Vyřazení zařízení a Vymazání zařízení můžete použít k odebrání firemních dat spravovaných Intune nebo k obnovení továrního nastavení a k návratu zařízení do výchozího nastavení.

1. Přihlaste se Microsoft 365 zařízení a přejděte na **Zařízení**  >  **všechna zařízení**.
2. Vyberte zařízení, které chcete vymazat.
3. Vyberte typ vzdáleného vymazání, které chcete udělat. Vyřazení odstraní jenom informace o organizaci, zatímco úplné vymazání zařízení obnoví do továrního nastavení.
4. Potvrďte **výběrem** možnosti Ano. Dokud se vymazání nedokončí, zobrazí se stav akce Zařízení jako *Čeká na vyřazení.*
    Po dokončení akce se už mobilní zařízení v seznamu spravovaných zařízení neuvidí.

**Poznámka:** Data společnosti nelze odebrat ze zařízení SPOJENÝch se službou Azure AD. 

Úplné podrobnosti o účinku akcí Vyřazení a vymazání, včetně toho, co je zachované a co se odstraní, najdete v následující dokumentaci:

- [Odeberte zařízení pomocí vymazání, vyřazení](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)nebo ručního zrušení registrace zařízení .
- [Jak vymazat jenom podniková data z aplikací spravovaných Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Vymažte všechna data ze zařízení s macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).