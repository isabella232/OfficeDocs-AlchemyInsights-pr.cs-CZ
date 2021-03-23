---
title: Volného místa na disku ve Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035668"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="aa60f-102">Volného místa na disku ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="aa60f-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="aa60f-103">Tady jsou dvě možnosti, jak ve Windows volného místa na disku:</span><span class="sxs-lookup"><span data-stu-id="aa60f-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="aa60f-104">Volná místa na disku ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="aa60f-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="aa60f-105">Volná místa pro aktualizace Windows 10 s externím úložným zařízením</span><span class="sxs-lookup"><span data-stu-id="aa60f-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="aa60f-106">Pokud máte po použití nástroje Vyčištění disku pořád málo místa na disku, je možné, že složka Temp se rychle zaplní soubory aplikací (.appx), které používá Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="aa60f-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="aa60f-107">Pokud chcete tento problém vyřešit, obnovte Store, vymažte mezipaměť Storu a spusťte Poradce při potížích se službou Windows Update.</span><span class="sxs-lookup"><span data-stu-id="aa60f-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="aa60f-108">Než budete pokračovat v těchto krocích, ujistěte se, že je Microsoft Store zavřený.</span><span class="sxs-lookup"><span data-stu-id="aa60f-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="aa60f-109">**Krok 1: Resetování Microsoft Storu**</span><span class="sxs-lookup"><span data-stu-id="aa60f-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="aa60f-110">**Poznámka:** Tím se trvale odstraní data aplikace na zařízení, včetně vašich předvoleb a přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="aa60f-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="aa60f-111">Vyberte **Start**  >  **Settings**  >  **Apps**  >  **Apps & funkce**.</span><span class="sxs-lookup"><span data-stu-id="aa60f-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="aa60f-112">V seznamu aplikací vyhledejte a vyberte Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="aa60f-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="aa60f-113">Vyberte **Upřesnit možnosti**.</span><span class="sxs-lookup"><span data-stu-id="aa60f-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="aa60f-114">Posuňte se dolů, **vyberte Obnovit a** pak **Potvrdit obnovení továrního nastavení.**</span><span class="sxs-lookup"><span data-stu-id="aa60f-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="aa60f-115">**Krok 2: Vymazání mezipaměti Microsoft Storu**</span><span class="sxs-lookup"><span data-stu-id="aa60f-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="aa60f-116">Stisknutím klávesy s logem Windows + R otevřete dialogové okno Spustit.</span><span class="sxs-lookup"><span data-stu-id="aa60f-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="aa60f-117">Zadejte wsreset.exe a vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa60f-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="aa60f-118">Otevře se prázdné okno příkazového řádku.</span><span class="sxs-lookup"><span data-stu-id="aa60f-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="aa60f-119">Po přibližně 10 sekundách se okno zavře a Store se otevře automaticky.</span><span class="sxs-lookup"><span data-stu-id="aa60f-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="aa60f-120">**Krok 3: Resetování služby Windows Update**</span><span class="sxs-lookup"><span data-stu-id="aa60f-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="aa60f-121">Vyberte **Spustit**  >  **aktualizace nastavení** a & poradce při  >  **potížích se**  >  **zabezpečením**.</span><span class="sxs-lookup"><span data-stu-id="aa60f-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="aa60f-122">Posuňte se dolů a v seznamu vyberte **Windows Update** a vyberte Spustit poradce **při potížích.**</span><span class="sxs-lookup"><span data-stu-id="aa60f-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="aa60f-123">Restartujte počítač a zkontrolujte, jestli k problému stále dochází.</span><span class="sxs-lookup"><span data-stu-id="aa60f-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

