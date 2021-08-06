---
title: Spusťte Windows diagnostika paměti v Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922519"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Spusťte Windows diagnostika paměti v Windows 10

Pokud Windows a aplikace na počítači havarují, zamrznou nebo působí nestabilním způsobem, můžete mít problém s pamětí POČÍTAČE (RAM). Spuštěním nástroje Windows Paměti můžete zkontrolovat problémy s pamětí RAM počítače.

Do vyhledávacího pole na hlavním panelu zadejte **diagnostika** paměti a pak vyberte **Windows Diagnostika paměti**. 

Pokud chcete spustit diagnostiku, musí se počítač restartovat. Máte možnost okamžitě restartovat (uložte si prosím svou práci a zavřete nejdřív otevřené dokumenty a e-maily), nebo naplánujte automatické spuštění diagnostiky při příštím restartování počítače:

![Windows Diagnostika paměti](media/windows-memory-diagnostic.png)

Po restartování počítače se **nástroj Windows paměti** automaticky spustí. Stav a průběh se zobrazí při spuštění diagnostiky a máte možnost diagnostiku zrušit stisknutím klávesy **ESC** na klávesnici.

Po dokončení diagnostiky se Windows normálně.
Hned po restartování se po zobrazení plochy zobrazí oznámení (vedle ikony **Centra** akcí na hlavním panelu), které označuje, jestli byly nalezeny nějaké chyby paměti. Příklad:

Tady je ikona Centra akcí: ![Ikona Centra akcí](media/action-center-icon.png) 

A ukázkové oznámení: ![Žádné chyby paměti](media/no-memory-errors.png)

Pokud jste oznámení zmeškali, můžete na hlavním panelu  vybrat ikonu Centrum akcí a zobrazit tak posuvný seznam oznámení. 

Pokud chcete zobrazit podrobné informace, **zadejte událost** do vyhledávacího pole na hlavním panelu a pak vyberte **Prohlížeč událostí**. V levém **podokně Prohlížeče** událostí přejděte na Windows Protokoly **> Systému**. V pravém podokně naskenujte seznam dolů  a podívejte se na sloupec Zdroj, dokud neuvidíte události se zdrojovou hodnotou **MemoryDiagnostics-Results**. Zvýrazněte každou takovou událost a podívejte se na informace o výsledku v poli **na** kartě Obecné pod seznamem.
