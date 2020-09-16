---
title: Spuštění diagnostiky paměti Windows ve Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720783"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="faa41-102">Spuštění diagnostiky paměti Windows ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="faa41-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="faa41-103">Pokud systém Windows a aplikace na vašem počítači způsobí zhroucení, mrznutí nebo nestabilní způsob, může dojít k potížím s pamětí počítače (RAM).</span><span class="sxs-lookup"><span data-stu-id="faa41-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="faa41-104">Nástroj Diagnostika paměti Windows můžete použít ke kontrole problémů s pamětí RAM počítače.</span><span class="sxs-lookup"><span data-stu-id="faa41-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="faa41-105">Do vyhledávacího pole na hlavním panelu zadejte **Diagnostika paměti**a pak vyberte **Nástroj Diagnostika paměti Windows**.</span><span class="sxs-lookup"><span data-stu-id="faa41-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="faa41-106">Pokud chcete diagnostiku spustit, musí se počítač restartovat.</span><span class="sxs-lookup"><span data-stu-id="faa41-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="faa41-107">Máte možnost okamžitě restartovat (uložte svoji práci a zavřete otevřené dokumenty a e-maily), nebo naplánujte automatické spuštění diagnostiky při příštím restartování počítače:</span><span class="sxs-lookup"><span data-stu-id="faa41-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Memory Diagnostic](media/windows-memory-diagnostic.png)

<span data-ttu-id="faa41-109">Po restartování počítače se automaticky spustí **Nástroj Diagnostika paměti Windows** .</span><span class="sxs-lookup"><span data-stu-id="faa41-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="faa41-110">Stav a průběh se zobrazí jako diagnostický nástroj a máte možnost, abyste diagnostiku zrušili stisknutím klávesy **ESC** na klávesnici.</span><span class="sxs-lookup"><span data-stu-id="faa41-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="faa41-111">Po dokončení diagnostiky se systém Windows spustí normálně.</span><span class="sxs-lookup"><span data-stu-id="faa41-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="faa41-112">Hned po restartování po zobrazení plochy se zobrazí oznámení (vedle ikony **Centrum akcí** na hlavním panelu), které označuje, jestli byly nalezeny nějaké chyby paměti.</span><span class="sxs-lookup"><span data-stu-id="faa41-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="faa41-113">Příklad:</span><span class="sxs-lookup"><span data-stu-id="faa41-113">For example:</span></span>

<span data-ttu-id="faa41-114">Tady je ikona centra akcí:</span><span class="sxs-lookup"><span data-stu-id="faa41-114">Here's the Action Center icon:</span></span> ![Ikona centra akcí](media/action-center-icon.png) 

<span data-ttu-id="faa41-116">A ukázkové oznámení:</span><span class="sxs-lookup"><span data-stu-id="faa41-116">And a sample notification:</span></span> ![Žádné chyby paměti](media/no-memory-errors.png)

<span data-ttu-id="faa41-118">Pokud jste oznámení zmeškali, můžete vybrat ikonu **centra akcí** na hlavním panelu a zobrazit **Centrum akcí** a zobrazit posuvný seznam oznámení.</span><span class="sxs-lookup"><span data-stu-id="faa41-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="faa41-119">Podrobné informace zobrazíte tak, že do vyhledávacího pole na hlavním panelu zadáte **událost** a pak vyberete **Prohlížeč událostí**.</span><span class="sxs-lookup"><span data-stu-id="faa41-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="faa41-120">V levém podokně **prohlížeče událostí**přejděte na **protokoly Windows > systém**.</span><span class="sxs-lookup"><span data-stu-id="faa41-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="faa41-121">V pravém podokně prohledejte seznam ve **zdrojovém** sloupci, dokud neuvidíte události se zdrojovou hodnotou **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="faa41-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="faa41-122">Zvýrazněte každou událost a podívejte se na informace o výsledku do pole pod kartou **Obecné** pod seznamem.</span><span class="sxs-lookup"><span data-stu-id="faa41-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
