---
title: 'Chyba: pravidla na tomto počítači se neshodují.'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690956"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: pravidla na tomto počítači se neshodují.

Pokud chcete zobrazit aktualizovaný stav tohoto známého problému, přečtěte si článek [pravidla na tomto počítači se neshodují s pravidly na serveru Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) .

Tým Outlooku implementoval opravu v buildu 12928,10000. Oprava už je v programu Insider Fast a přejde na měsíční kanál v pozdní 2020. Jakmile budete mít pevné buildy, může se zobrazit výzva "která pravidla chcete uchovat". Po zobrazení výzvy zvolte server a pak se vraťte v Outlooku a znovu povolte všechna pravidla, která byla zakázána.

Dokud nebude oprava k dispozici, použijte následující alternativní řešení:

**Alternativní řešení**: v seznamu nedávné sestavy se vyskytl problém u těch, které mají v Outlooku na počítači jenom vytvořená klientská pravidla. Pokud se problém pořád začne používat, zvažte odstranění pravidel a pak pravidla vytvořte a upravte jenom v OWA (Outlook Web Appu), dokud se problém nevyřeší.

Pokud nemůžete pravidla odstranit ručně, můžete při spuštění Outlooku spuštěním Outlook.exe/cleanrules. spustit příkaz Outlook Tato akce odstraní pravidla klienta i serveru. Odstraní všechna pravidla všech účtů v profilu Outlooku. Tento příkaz je dále zdokumentován v článku přepínače příkazového řádku.

