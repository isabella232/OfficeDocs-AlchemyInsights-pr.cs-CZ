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
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="8541e-102">Chyba: Pravidla v tomto počítači se neshodují</span><span class="sxs-lookup"><span data-stu-id="8541e-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="8541e-103">Aktualizovaný stav tohoto známého problému naleznete v [tématu Pravidla v tomto počítači neodpovídají pravidlům na serveru Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="8541e-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="8541e-104">Tým aplikace Outlook implementoval opravu v sestavení 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="8541e-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="8541e-105">Oprava je již na Insider Fast a půjde do Měsíční kanál na konci června 2020.</span><span class="sxs-lookup"><span data-stu-id="8541e-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="8541e-106">Jakmile budete mít pevné sestavení, můžete naposledy zobrazit výzvu "Která pravidla chcete zachovat".</span><span class="sxs-lookup"><span data-stu-id="8541e-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="8541e-107">Po zobrazení výzvy zvolte Server a pak se vraťte do aplikace Outlook a znovu povolte všechna pravidla, která byla zakázána.</span><span class="sxs-lookup"><span data-stu-id="8541e-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="8541e-108">Dokud nebude oprava k dispozici, použijte následující řešení:</span><span class="sxs-lookup"><span data-stu-id="8541e-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="8541e-109">**Řešení:** V posledních sestavách došlo k problému u těch, kteří vytvořili pouze pravidla klienta na ploše aplikace Outlook.</span><span class="sxs-lookup"><span data-stu-id="8541e-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="8541e-110">Pokud se na problém nadále navážáte, zvažte odstranění pravidel a potom vytvořte a upravte pravidla jenom v aplikaci OWA (Outlook Web App), dokud se problém nevyřeší.</span><span class="sxs-lookup"><span data-stu-id="8541e-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="8541e-111">Pokud nemůžete odstranit pravidla ručně, můžete spustit příkaz aplikace Outlook při spuštění aplikace Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="8541e-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="8541e-112">Tím odstraníte pravidla klienta i serveru.</span><span class="sxs-lookup"><span data-stu-id="8541e-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="8541e-113">Odstraní všechna pravidla pro všechny účty v profilu aplikace Outlook.</span><span class="sxs-lookup"><span data-stu-id="8541e-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="8541e-114">Tento příkaz je dále dokumentován v článku přepínače příkazového řádku.</span><span class="sxs-lookup"><span data-stu-id="8541e-114">This command is further documented in the Command-line switches article.</span></span>

