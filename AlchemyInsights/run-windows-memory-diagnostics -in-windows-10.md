---
title: Spuštění diagnostiky paměti Windows ve Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720783"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Spuštění diagnostiky paměti Windows ve Windows 10

Pokud systém Windows a aplikace na vašem počítači způsobí zhroucení, mrznutí nebo nestabilní způsob, může dojít k potížím s pamětí počítače (RAM). Nástroj Diagnostika paměti Windows můžete použít ke kontrole problémů s pamětí RAM počítače.

Do vyhledávacího pole na hlavním panelu zadejte **Diagnostika paměti**a pak vyberte **Nástroj Diagnostika paměti Windows**. 

Pokud chcete diagnostiku spustit, musí se počítač restartovat. Máte možnost okamžitě restartovat (uložte svoji práci a zavřete otevřené dokumenty a e-maily), nebo naplánujte automatické spuštění diagnostiky při příštím restartování počítače:

![Windows Memory Diagnostic](media/windows-memory-diagnostic.png)

Po restartování počítače se automaticky spustí **Nástroj Diagnostika paměti Windows** . Stav a průběh se zobrazí jako diagnostický nástroj a máte možnost, abyste diagnostiku zrušili stisknutím klávesy **ESC** na klávesnici.

Po dokončení diagnostiky se systém Windows spustí normálně.
Hned po restartování po zobrazení plochy se zobrazí oznámení (vedle ikony **Centrum akcí** na hlavním panelu), které označuje, jestli byly nalezeny nějaké chyby paměti. Příklad:

Tady je ikona centra akcí: ![Ikona centra akcí](media/action-center-icon.png) 

A ukázkové oznámení: ![Žádné chyby paměti](media/no-memory-errors.png)

Pokud jste oznámení zmeškali, můžete vybrat ikonu **centra akcí** na hlavním panelu a zobrazit **Centrum akcí** a zobrazit posuvný seznam oznámení.

Podrobné informace zobrazíte tak, že do vyhledávacího pole na hlavním panelu zadáte **událost** a pak vyberete **Prohlížeč událostí**. V levém podokně **prohlížeče událostí**přejděte na **protokoly Windows > systém**. V pravém podokně prohledejte seznam ve **zdrojovém** sloupci, dokud neuvidíte události se zdrojovou hodnotou **MemoryDiagnostics-Results**. Zvýrazněte každou událost a podívejte se na informace o výsledku do pole pod kartou **Obecné** pod seznamem.
