---
title: Vyhledání ztracených zařízení s iOS pomocí Intune
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
ms.openlocfilehash: af747a63caf76e7b4a4a180eaef25dfdf2cb5e3391079c713fe0e413198efb15
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042299"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Vyhledání ztracených zařízení s iOS pomocí Intune

Povolení režimu ztráty na zařízení s iOSem umožňuje správci zobrazit na zamykací obrazovce zprávu a telefonní číslo kontaktu.

Po povolení režimu ztráty může správce použít akci Vyhledat zařízení k identifikaci fyzického umístění zařízení.

Akce Vyhledat zařízení v Intune funguje se zařízeními s iOSem a zobrazí umístění konkrétního zařízení na mapě.

Použití této akce vyžaduje, aby zařízení s iOSem bylo v:

- Režim dohledu
- Režim ztráty

Další informace najdete v článku Povolení režimu ztráty na zařízeních [s iOS/iPadOS](https://docs.microsoft.com/intune/device-lost-mode) pomocí Intune a Vyhledání ztracených nebo odcizených zařízení [s iOS/iPadOS pomocí Intune](https://docs.microsoft.com/intune/device-locate).

**Nejčastější dotazy**

Otázka: Vydal(a) jsem vzdálenou akci pro odebrání firemních dat ze zařízení a teď je zaseknutá v čekajícím stavu.

A: Aby se vzdálená akce úspěšně dokončila, musí být cílové zařízení online a v pořádku. V následujících situacích zůstane vzdálená akce v čekajícím stavu po dobu 30 dnů nebo dokud zařízení tento příkaz nepotvrzí:

- Pokud zařízení nemá připojení
- Když zařízení ztratí stav správy v Intune

Pokud si myslíte, že se už zařízení neschová a že nebude moct data společnosti odebrat, vyberte Odstranit. Odstraněním odeberete záznam zařízení, aby se už v seznamu zařízení Intune nezobrazí. Pokud se zařízení znovu stane aktivním, bude ho muset uživatel znovu zaregistrovat.

Otázka: Proč nejsou některé vzdálené akce pro mě dostupné?

A: Všechny akce vzdáleného zařízení nepodporují všechny platformy. Následující vzdálené akce jsou specifické pro platformu, takže jsou dostupné jenom pro platformy.

- Obejití zámku aktivace (jenom v systému iOS)
- Fresh Start (pouze Windows)
- Režim ztráty (jenom v iOSu)
- Vyhledání zařízení (jenom v iOSu)
- Restartování (jenom Windows)

Další informace o jednotlivých akcích najdete v tématu [Dostupné akce zařízení](https://docs.microsoft.com/intune/device-management#available-device-actions).