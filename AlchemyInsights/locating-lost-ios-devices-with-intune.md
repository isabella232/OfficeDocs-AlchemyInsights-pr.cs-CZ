---
title: Vyhledání ztracených zařízení s iOS s Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675149"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Vyhledání ztracených zařízení s iOS s Intune

Povolení režimu ztráty na zařízení s iOS umožňuje správci na zamykací obrazovce zobrazit zprávu a telefonní číslo.

Když je režim ztráty povolený, může správce pomocí akce najít zařízení identifikovat fyzické umístění zařízení.

Akce najít zařízení v Intune funguje se zařízeními s iOS, která ukazuje umístění určitého zařízení na mapě.

Použití této akce vyžaduje, aby bylo zařízení s iOS v:

- Sledovaný režim
- Režim ztráty

Další informace najdete v článku [Povolení režimu ztraceného zobrazení na zařízeních s iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-lost-mode) a [vyhledání ztracených nebo odcizených zařízení s iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-locate).

**Nejčastější dotazy**

Otázka: byla vydána vzdálená akce, která odebere firemní data ze zařízení a teď je ve stavu čekání na vyřízení.

A: aby byla úspěšná vzdálená akce, musí být cílové zařízení online a v pořádku. V následujících situacích zůstane vzdálená akce v nevyřízeném stavu po dobu 30 dnů nebo dokud zařízení nepotvrdí příkaz:

- Pokud zařízení nemá připojení
- Když zařízení ztratí stav správy s Intune

Pokud si myslíte, že zařízení už není v nerezervování, a že nepůjde odebrat data společnosti, vyberte Odstranit. Odstraněním odeberete záznam zařízení, aby se už nezobrazoval v seznamu zařízení v Intune. Pokud se zařízení opět stane aktivní, bude ho muset uživatel znovu zaregistrovat.

Otázka: Proč nejsou některé vzdálené akce pro mě k dispozici?

A: ne všechny platformy podporují všechny akce vzdálených zařízení. Následující vzdálené akce jsou závislé na platformě, takže jsou k dispozici pouze pro uvedené platformy.

- Vynechat zámek aktivace (jenom iOS)
- Nové spuštění (jenom Windows)
- Ztracené zobrazení (jenom iOS)
- Vyhledání zařízení (jenom iOS)
- Restartovat (jenom Windows)

Další podrobnosti o jednotlivých akcích najdete v tématu [Dostupné akce zařízení](https://docs.microsoft.com/intune/device-management#available-device-actions).