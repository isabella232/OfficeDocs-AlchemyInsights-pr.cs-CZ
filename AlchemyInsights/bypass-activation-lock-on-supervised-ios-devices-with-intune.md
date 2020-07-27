---
title: Obejít zámek aktivace na kontrolovaných zařízeních iOS s Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423490"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Obejít zámek aktivace na kontrolovaných zařízeních iOS s Intune

Možnost obejít zámek aktivace na zařízeních se systémem iOS usnadňuje obnovení ze scénáře, kdy uživatel povolí zámek aktivace na podnikovém zařízení a pak opustí společnost.

Předpoklady k vynechání zámku aktivace zahrnují:

- Zařízení je, že je "pod dohledem."
- Zámek aktivace je úspěšně povolený pomocí zásad omezení zařízení iOS v Intune.

Kromě toho při vynechání zámku aktivace byste měli:

- Fyzicky ovládni zařízení, které bylo vymazáno.
- Před vydáním vymazání zkopírujte kód.

**Poznámka:** Kód vymazání nerozlišuje malá a velká písmena, takže znaky "-" nejsou vyžadovány.

Podrobnosti najdete v [tématu Vynechání zámku aktivace na zařízeních s iOS s Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Nejčastější dotazy**

Otázka: **Vydal jsem vzdálenou akci k odebrání firemních dat ze zařízení a nyní se zasekne ve stavu čekající na vyřízení.**

A: Pro vzdálené akce úspěšně dokončit cílové zařízení musí být online a v pořádku. V následujících situacích zůstane vzdálená akce ve stavu čekající na vyřízení po dobu 30 dnů nebo dokud zařízení nepotvrdí příkaz, když zařízení:

- Nemá připojení.
- Ztratí svůj stav správy s Intune.

Pokud se domníváte, že zařízení se už nehlásí a že neodebere firemní data, vyberte Odstranit. Odstraněním odeberete záznam zařízení, aby se už nezobával v seznamu zařízení Intune. Aby se zařízení znovu aktivovalo, musí jeho uživatel zařízení znovu zaregistrovat.

Otázka: **Proč nejsou k dispozici určité vzdálené akce, které nelze použít?**

A: Ne všechny platformy podporují všechny akce vzdáleného zařízení. Následující vzdálené akce jsou specifické pro platformu.

- Vynechání zámku aktivace (pouze iOS)
- Nový začátek (pouze windows)
- Režim ztráty (pouze iOS)
- Vyhledání zařízení (pouze iOS)
- Restartování (pouze windows)

Další podrobnosti o jednotlivých akcích najdete v [tématu Dostupné akce zařízení](https://docs.microsoft.com/intune/device-management#available-device-actions).