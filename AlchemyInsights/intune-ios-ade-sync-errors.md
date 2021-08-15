---
title: Chyby synchronizace automatického zápisu zařízení Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013741"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Chyby synchronizace automatického zápisu zařízení Apple

"Zjistili jsme, že máte jeden nebo více tokenů ADE/DEP, které jsou v chybovém stavu. Dokud se u každého ovlivněného tokenu nevyřeší stav chyby, nebude funkce ADE fungovat očekávaným způsobem."

Tato chyba se může projevit několika způsoby, například:

1. Zařízení se nemusí synchronizovat z ABM/ASM do Intune.
2. Přiřazení profilu registrace se možná nedaří.
3. Zařízení nemusí úspěšně dokončit registraci ADE.

Zkontrolujte, zda se v konzole Intune nehlásila chyba synchronizace v části Zařízení > Zaregistrovat zařízení **> apple > programové tokeny**.

Jednou z nejčastějších příčin chyby synchronizace je vypršení platnosti aktuálního tokenu. V mnoha případech se problém vyřeší obnovením ovlivněného tokenu.

Pokud vypršela platnost jednoho nebo více tokenů, podívejte se do následující dokumentace, která vám pomůže je podle potřeby prodloužit:

[Prodloužení tokenu automatického zápisu zařízení](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Kromě toho se můžete podívat na následující dokumentaci a zobrazit potenciální opravy dalších chyb způsobujících selhání synchronizace tokenů:

[Chyby synchronizace ABM/ASM pro iOS/iPadOS a macOS – automatické tokeny registrace zařízení](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Chyby synchronizace ABM/ASM pro iOS/iPadOS a macOS – automatické tokeny registrace zařízení](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
