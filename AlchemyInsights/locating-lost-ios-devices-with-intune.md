---
title: Vyhledání ztracených zařízení iOS pomocí Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439145"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Vyhledání ztracených zařízení iOS pomocí Intune

Povolení režimu ztráty na zařízení se systémem iOS umožňuje správci zobrazit na zamykací obrazovce zprávu a telefonní číslo kontaktu.

Po povolení režimu ztráty může správce použít akci Vyhledat zařízení k identifikaci fyzického umístění zařízení.

Akce Najít zařízení v Intune funguje se zařízeními s iOS a zobrazuje umístění konkrétního zařízení na mapě.

Použití této akce vyžaduje, aby se iOS zařízení nachyoduje v:

- Režim pod dohledem
- Režim ztráty

Další informace najdete v [tématu Povolení režimu ztráty na zařízeních iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-lost-mode) a [Vyhledání ztracených nebo odcizených zařízení iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-locate).

**Nejčastější dotazy**

Otázka: Vydal jsem vzdálenou akci k odebrání firemních dat ze zařízení a nyní se zasekne ve stavu čekající na vyřízení.

A: Pro vzdálené akce úspěšně dokončit cílové zařízení musí být online a v pořádku. V následujících situacích zůstane vzdálená akce ve stavu čekající na vyřízení po dobu 30 dnů nebo dokud zařízení příkaz nepotvrdí:

- Pokud zařízení nemá připojení
- Když zařízení ztratí svůj stav správy s Intune

Pokud se domníváte, že zařízení se už nehlásí a že nebude moct odebrat firemní data, vyberte Odstranit. Odstraněním odeberete záznam zařízení, aby se už nezobával v seznamu zařízení Intune. Pokud se zařízení znovu aktivuje, jeho uživatel jej bude muset znovu zaregistrovat.

Otázka: Proč nejsou k dispozici určité vzdálené akce, které nelze použít?

A: Ne všechny platformy podporují všechny akce vzdáleného zařízení. Následující vzdálené akce jsou specifické pro platformu, takže jsou k dispozici pouze pro uvedené platformy.

- Vynechání zámku aktivace (pouze iOS)
- Nový začátek (pouze windows)
- Režim ztráty (pouze iOS)
- Vyhledání zařízení (pouze iOS)
- Restartování (pouze windows)

Další podrobnosti o jednotlivých akcích najdete v [tématu Dostupné akce zařízení](https://docs.microsoft.com/intune/device-management#available-device-actions).