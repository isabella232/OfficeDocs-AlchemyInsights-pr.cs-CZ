---
title: 'Chyba: Pravidla na tomto počítači se neshodují'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782945"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: Pravidla na tomto počítači se neshodují

Pokud chcete zobrazit aktualizovaný stav tohoto známého problému, podívejte se na článek Pravidla na tomto počítači neodpovídají pravidlům [v Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tým Outlooku implementovali opravu v buildu 12928.10000. Oprava už je v programu Insider Fast a na konci června 2020 půjde do Měsíčního kanálu. Až budete mít opravený build, může se vám naposledy zobrazit výzva , která pravidla chcete zachovat. Po zobrazení výzvy zvolte Server a pak se vraťte do Outlooku a znovu povolte pravidla, která byla zakázaná.

Dokud nebude oprava dostupná, použijte následující alternativní řešení:

**Alternativní** řešení: V posledních sestavách došlo k problému u těch, kteří vytvořili pravidla klienta jenom v desktopové verzi Outlooku. Pokud se k problému budete i nadále dostat, zvažte odstranění pravidel a potom pravidla vytvořte a upravte jenom v aplikaci OWA (Outlook Web App), dokud se problém nevyřeší.

Pokud nemůžete pravidla odstranit ručně, můžete spustit příkaz Outlooku při spuštění Outlooku spuštěním Outlook.exe /cleanrules. Tím se odstraní pravidla klienta i serveru. Odstraní se všechna pravidla pro všechny účty v profilu Outlooku. Tento příkaz je dále zdokumentovaný v článku Přepínače příkazového řádku.

