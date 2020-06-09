---
title: 'Chyba: Pravidla v tomto počítači se neshodují'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664239"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: Pravidla v tomto počítači se neshodují

Aktualizovaný stav tohoto známého problému naleznete v [tématu Pravidla v tomto počítači neodpovídají pravidlům na serveru Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tým aplikace Outlook implementoval opravu v sestavení 12928.10000. Oprava je již na Insider Fast a půjde do Měsíční kanál na konci června 2020. Jakmile budete mít pevné sestavení, můžete naposledy zobrazit výzvu "Která pravidla chcete zachovat". Po zobrazení výzvy zvolte Server a pak se vraťte do aplikace Outlook a znovu povolte všechna pravidla, která byla zakázána.

Dokud nebude oprava k dispozici, použijte následující řešení:

**Řešení:** V posledních sestavách došlo k problému u těch, kteří vytvořili pouze pravidla klienta na ploše aplikace Outlook. Pokud se na problém nadále navážáte, zvažte odstranění pravidel a potom vytvořte a upravte pravidla jenom v aplikaci OWA (Outlook Web App), dokud se problém nevyřeší.

Pokud nemůžete odstranit pravidla ručně, můžete spustit příkaz aplikace Outlook při spuštění aplikace Outlook.exe /cleanrules. Tím odstraníte pravidla klienta i serveru. Odstraní všechna pravidla pro všechny účty v profilu aplikace Outlook. Tento příkaz je dále dokumentován v článku přepínače příkazového řádku.

