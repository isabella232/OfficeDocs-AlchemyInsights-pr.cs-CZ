---
title: Chyby při synchronizaci automatické registrace zařízení Apple
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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448915"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Chyby při synchronizaci automatické registrace zařízení Apple

"Zjistili jsme, že máte jeden nebo víc tokenů ADE/DEP, které jsou v chybovém stavu. Dokud se problém nevyřeší u každého ovlivněného tokenu, nebude funkce ADE fungovat podle očekávání."

Tato chyba se může projevit několika způsoby, mezi které patří:

1. Zařízení se nemusí synchronizovat z ABM/ASM do Intune
2. Zadání v profilu prováděcí smlouvy nemusí být neúspěšná
3. Zařízení nemusí úspěšně dokončovat registraci ADE.

Zkontrolujte, že v konzole Intune nehlásila chyba synchronizace v části **Zařízení > Enroll Devices > Apple enrollment > Enrollment program tokens**.

Jednou z nejčastějších příčin chyby synchronizace je vypršení platnosti aktuálního tokenu. V mnoha případech se problém vyřeší obnovením ovlivněného tokenu.

Pokud vypršela platnost jednoho nebo více vašich tokenů, podívejte se do následující dokumentace, abyste si je podle potřeby pomohli obnovit:

[Prodloužení automatického registračního tokenu zařízení](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Kromě toho si můžete zobrazit následující dokumentaci, abyste se mohli podívat na možná řešení jiných chyb, které způsobují chyby synchronizace tokenů:

[Chyby synchronizace ABM/ASM pro iOS/iPadOS a macOS automated device enrollment tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Chyby synchronizace ABM/ASM pro iOS/iPadOS a macOS automated device enrollment tokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
