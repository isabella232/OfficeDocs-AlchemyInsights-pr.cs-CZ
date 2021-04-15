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
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="3e9ec-102">Chyba: Pravidla na tomto počítači se neshodují</span><span class="sxs-lookup"><span data-stu-id="3e9ec-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="3e9ec-103">Pokud chcete zobrazit aktualizovaný stav tohoto známého problému, podívejte se na článek Pravidla na tomto počítači neodpovídají pravidlům [v Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="3e9ec-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="3e9ec-104">Tým Outlooku implementovali opravu v buildu 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="3e9ec-105">Oprava už je v programu Insider Fast a na konci června 2020 půjde do Měsíčního kanálu.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="3e9ec-106">Až budete mít opravený build, může se vám naposledy zobrazit výzva , která pravidla chcete zachovat.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="3e9ec-107">Po zobrazení výzvy zvolte Server a pak se vraťte do Outlooku a znovu povolte pravidla, která byla zakázaná.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="3e9ec-108">Dokud nebude oprava dostupná, použijte následující alternativní řešení:</span><span class="sxs-lookup"><span data-stu-id="3e9ec-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="3e9ec-109">**Alternativní** řešení: V posledních sestavách došlo k problému u těch, kteří vytvořili pravidla klienta jenom v desktopové verzi Outlooku.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="3e9ec-110">Pokud se k problému budete i nadále dostat, zvažte odstranění pravidel a potom pravidla vytvořte a upravte jenom v aplikaci OWA (Outlook Web App), dokud se problém nevyřeší.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="3e9ec-111">Pokud nemůžete pravidla odstranit ručně, můžete spustit příkaz Outlooku při spuštění Outlooku spuštěním Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="3e9ec-112">Tím se odstraní pravidla klienta i serveru.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="3e9ec-113">Odstraní se všechna pravidla pro všechny účty v profilu Outlooku.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="3e9ec-114">Tento příkaz je dále zdokumentovaný v článku Přepínače příkazového řádku.</span><span class="sxs-lookup"><span data-stu-id="3e9ec-114">This command is further documented in the Command-line switches article.</span></span>

