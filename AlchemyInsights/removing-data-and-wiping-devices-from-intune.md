---
title: Odebrání dat a vymazání zařízení z Intune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701276"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odebrání dat a vymazání zařízení z Intune

Odřazení zařízení a vymazání zařízení: vzdálené akce mohou být použity k odebrání dat společnosti spravovaných intunem nebo k provedení továrního resetu a obnovení výchozího nastavení zařízení.

1. Přihlaste se ke správě zařízení Microsoft 365 a **přejděte na**  >  **všechna zařízení**.
2. Vyberte zařízení, které chcete vymazat.
3. Vyberte typ vzdáleného vymazání, které chcete provést. Možnost vyřazení odstraní jenom informace o organizaci, zatímco možnost úplné vymazání zařízení obnoví do továrního nastavení.
4. Kliknutím na **Ano** potvrďte. Až do doby vymazání skončí, zobrazí se stav akce zařízení jako čekající vyřazení.</br>
    Po dokončení akce se v seznamu spravovaných zařízení už nezobrazuje mobilní zařízení.

**Poznámka:** Data společnosti nejde odebrat ze zařízení připojených k Azure AD.

Podrobné informace o vlivu akcí vyřazení a vymazání, včetně informací o tom, co je zachováno a o odstranění, najdete v tématu [odebrání zařízení pomocí vymazání, vyřazení nebo ručním odregistraci zařízení](https://docs.microsoft.com/intune/devices-wipe).

Pokud chcete vymazat všechna data ze zařízení macOS, přečtěte si článek [vymazání všech dat ze zařízení MacOS](https://docs.microsoft.com/intune/device-erase).