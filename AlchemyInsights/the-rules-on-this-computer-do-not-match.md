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
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="a1bd1-102">Chyba: pravidla na tomto počítači se neshodují.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="a1bd1-103">Pokud chcete zobrazit aktualizovaný stav tohoto známého problému, přečtěte si článek [pravidla na tomto počítači se neshodují s pravidly na serveru Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) .</span><span class="sxs-lookup"><span data-stu-id="a1bd1-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="a1bd1-104">Tým Outlooku implementoval opravu v buildu 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="a1bd1-105">Oprava už je v programu Insider Fast a přejde na měsíční kanál v pozdní 2020.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="a1bd1-106">Jakmile budete mít pevné buildy, může se zobrazit výzva "která pravidla chcete uchovat".</span><span class="sxs-lookup"><span data-stu-id="a1bd1-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="a1bd1-107">Po zobrazení výzvy zvolte server a pak se vraťte v Outlooku a znovu povolte všechna pravidla, která byla zakázána.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="a1bd1-108">Dokud nebude oprava k dispozici, použijte následující alternativní řešení:</span><span class="sxs-lookup"><span data-stu-id="a1bd1-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="a1bd1-109">**Alternativní řešení**: v seznamu nedávné sestavy se vyskytl problém u těch, které mají v Outlooku na počítači jenom vytvořená klientská pravidla.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="a1bd1-110">Pokud se problém pořád začne používat, zvažte odstranění pravidel a pak pravidla vytvořte a upravte jenom v OWA (Outlook Web Appu), dokud se problém nevyřeší.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="a1bd1-111">Pokud nemůžete pravidla odstranit ručně, můžete při spuštění Outlooku spuštěním Outlook.exe/cleanrules. spustit příkaz Outlook</span><span class="sxs-lookup"><span data-stu-id="a1bd1-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="a1bd1-112">Tato akce odstraní pravidla klienta i serveru.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="a1bd1-113">Odstraní všechna pravidla všech účtů v profilu Outlooku.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="a1bd1-114">Tento příkaz je dále zdokumentován v článku přepínače příkazového řádku.</span><span class="sxs-lookup"><span data-stu-id="a1bd1-114">This command is further documented in the Command-line switches article.</span></span>

