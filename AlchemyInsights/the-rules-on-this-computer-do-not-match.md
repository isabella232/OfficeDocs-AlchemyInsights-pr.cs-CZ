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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981106"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: Pravidla na tomto počítači se neshodují

Pokud chcete zobrazit aktualizovaný stav tohoto známého problému, podívejte se na článek Pravidla na tomto počítači neodpovídají pravidlům [na webu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tým Outlook implementovali opravu v buildu 12928.10000. Oprava už je v programu Insider Fast a na konci června 2020 půjde do Měsíčního kanálu. Až budete mít opravený build, může se vám naposledy zobrazit výzva , která pravidla chcete zachovat. Po zobrazení výzvy zvolte Server a pak se vraťte do Outlook a znovu povolte pravidla, která byla zakázaná.

Dokud nebude oprava dostupná, použijte následující alternativní řešení:

**Alternativní** řešení: V posledních sestavách došlo k problému u těch, kteří vytvořili pravidla klienta jenom v Outlook desktopové verzi. Pokud se k problému budete dál dostat, zvažte odstranění pravidel a potom pravidla vytvořte a upravte jenom v aplikaci OWA (Outlook Web App), dokud se problém nevyřeší.

Pokud pravidla nemůžete odstranit ručně, můžete spustit příkaz Outlook při spuštění Outlook spuštěním příkazu Outlook.exe /cleanrules. Tím se odstraní pravidla klienta i serveru. Odstraní se všechna pravidla pro všechny účty v Outlook profilu. Tento příkaz je dále zdokumentovaný v článku Přepínače příkazového řádku.

