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
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="466df-102">Spuštění diagnostiky paměti Windows ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="466df-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="466df-103">Pokud windows a aplikace na vašem počítači dochází k chybě, zamrznutí nebo se chová nestabilním způsobem, můžete mít problém s pamětí POČÍTAČE (RAM).</span><span class="sxs-lookup"><span data-stu-id="466df-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="466df-104">Pokud chcete zjistit problémy s pamětí RAM počítače, můžete spustit Nástroj Windows Memory Diagnostic.</span><span class="sxs-lookup"><span data-stu-id="466df-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="466df-105">Do vyhledávacího pole na hlavním panelu zadejte **diagnostika paměti** a pak vyberte Diagnostika paměti **systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="466df-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="466df-106">Pokud chcete spustit diagnostiku, musí se počítač restartovat.</span><span class="sxs-lookup"><span data-stu-id="466df-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="466df-107">Máte možnost okamžitě restartovat (uložte si prosím svou práci a zavřete nejdřív otevřené dokumenty a e-maily), nebo naplánujte automatické spuštění diagnostiky při příštím restartování počítače:</span><span class="sxs-lookup"><span data-stu-id="466df-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostika paměti systému Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="466df-109">Po restartování počítače se nástroj **Windows Memory Diagnostics Tool** spustí automaticky.</span><span class="sxs-lookup"><span data-stu-id="466df-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="466df-110">Stav a průběh se zobrazí při spuštění diagnostiky a máte možnost diagnostiku zrušit stisknutím klávesy **ESC** na klávesnici.</span><span class="sxs-lookup"><span data-stu-id="466df-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="466df-111">Po dokončení diagnostiky se Systém Windows spustí normálně.</span><span class="sxs-lookup"><span data-stu-id="466df-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="466df-112">Hned po restartování se po zobrazení plochy zobrazí oznámení (vedle ikony **Centra** akcí na hlavním panelu), které označuje, jestli byly nalezeny nějaké chyby paměti.</span><span class="sxs-lookup"><span data-stu-id="466df-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="466df-113">Například:</span><span class="sxs-lookup"><span data-stu-id="466df-113">For example:</span></span>

<span data-ttu-id="466df-114">Tady je ikona Centra akcí:</span><span class="sxs-lookup"><span data-stu-id="466df-114">Here's the Action Center icon:</span></span> ![Ikona Centra akcí](media/action-center-icon.png) 

<span data-ttu-id="466df-116">A ukázkové oznámení:</span><span class="sxs-lookup"><span data-stu-id="466df-116">And a sample notification:</span></span> ![Žádné chyby paměti](media/no-memory-errors.png)

<span data-ttu-id="466df-118">Pokud jste oznámení zmeškali, můžete na hlavním panelu  vybrat ikonu Centrum akcí a zobrazit tak posuvný seznam oznámení. </span><span class="sxs-lookup"><span data-stu-id="466df-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="466df-119">Pokud chcete zobrazit podrobné informace, **zadejte událost** do vyhledávacího pole na hlavním panelu a pak vyberte **Prohlížeč událostí**.</span><span class="sxs-lookup"><span data-stu-id="466df-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="466df-120">V levém **podokně Prohlížeče** událostí přejděte na Protokoly systému Windows **> Systému**.</span><span class="sxs-lookup"><span data-stu-id="466df-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="466df-121">V pravém podokně naskenujte seznam dolů  a podívejte se na sloupec Zdroj, dokud neuvidíte události se zdrojovou hodnotou **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="466df-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="466df-122">Zvýrazněte každou takovou událost a podívejte se na informace o výsledku v poli **na** kartě Obecné pod seznamem.</span><span class="sxs-lookup"><span data-stu-id="466df-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
