---
title: Chyby synchronizace automatického zápisu zařízení Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714690"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Chyby synchronizace automatického zápisu zařízení Apple

Zjistili jsme, že máte jeden nebo víc tokenů ADE/DEP, které jsou v chybovém stavu. Dokud nebude chybový stav vyřešen u každého úspěšného tokenu, nebudou funkce ADE fungovat stejně.

Tato chyba může být v mnoha ohledech:

1. Zařízení se nemusí synchronizovat z ABM/ASM na Intune
2. Přiřazení profilu registrace se nemusí zdařit
3. Zařízení nemusí dokončit zápis ADE.

Zkontrolujte, jestli je chyba synchronizace hlášená v konzoli Intune v části **zařízení > zaregistrovat zařízení > tokeny programu Apple enrollment > pro zápis** , a podívejte se na následující dokumentaci, kde se zobrazí jakákoli potenciální Oprava:

[Chyby synchronizace ABM/ASM pro tokeny automatických zápisů s iOS/iPadOS a macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
