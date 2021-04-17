---
title: Spuštění diagnostiky paměti Windows ve Windows 10
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
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826660"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Spuštění diagnostiky paměti Windows ve Windows 10

Pokud windows a aplikace na vašem počítači dochází k chybě, zamrznutí nebo se chová nestabilním způsobem, můžete mít problém s pamětí POČÍTAČE (RAM). Pokud chcete zjistit problémy s pamětí RAM počítače, můžete spustit Nástroj Windows Memory Diagnostic.

Do vyhledávacího pole na hlavním panelu zadejte **diagnostika paměti** a pak vyberte Diagnostika paměti **systému Windows**. 

Pokud chcete spustit diagnostiku, musí se počítač restartovat. Máte možnost okamžitě restartovat (uložte si prosím svou práci a zavřete nejdřív otevřené dokumenty a e-maily), nebo naplánujte automatické spuštění diagnostiky při příštím restartování počítače:

![Diagnostika paměti systému Windows](media/windows-memory-diagnostic.png)

Po restartování počítače se nástroj **Windows Memory Diagnostics Tool** spustí automaticky. Stav a průběh se zobrazí při spuštění diagnostiky a máte možnost diagnostiku zrušit stisknutím klávesy **ESC** na klávesnici.

Po dokončení diagnostiky se Systém Windows spustí normálně.
Hned po restartování se po zobrazení plochy zobrazí oznámení (vedle ikony **Centra** akcí na hlavním panelu), které označuje, jestli byly nalezeny nějaké chyby paměti. Například:

Tady je ikona Centra akcí: ![Ikona Centra akcí](media/action-center-icon.png) 

A ukázkové oznámení: ![Žádné chyby paměti](media/no-memory-errors.png)

Pokud jste oznámení zmeškali, můžete na hlavním panelu  vybrat ikonu Centrum akcí a zobrazit tak posuvný seznam oznámení. 

Pokud chcete zobrazit podrobné informace, **zadejte událost** do vyhledávacího pole na hlavním panelu a pak vyberte **Prohlížeč událostí**. V levém **podokně Prohlížeče** událostí přejděte na Protokoly systému Windows **> Systému**. V pravém podokně naskenujte seznam dolů  a podívejte se na sloupec Zdroj, dokud neuvidíte události se zdrojovou hodnotou **MemoryDiagnostics-Results**. Zvýrazněte každou takovou událost a podívejte se na informace o výsledku v poli **na** kartě Obecné pod seznamem.
