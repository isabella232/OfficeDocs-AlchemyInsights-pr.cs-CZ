---
title: Uvolnění místa na disku ve Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505349"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="9d336-102">Uvolnění místa na disku ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="9d336-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="9d336-103">Tady jsou dvě možnosti, jak uvolnit místo na disku ve Windows:</span><span class="sxs-lookup"><span data-stu-id="9d336-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="9d336-104">Uvolnění místa na disku ve Windows 10.</span><span class="sxs-lookup"><span data-stu-id="9d336-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="9d336-105">Uvolněte místo pro aktualizace Windows 10 s pomocí externího úložiště.</span><span class="sxs-lookup"><span data-stu-id="9d336-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="9d336-106">Pokud máte po použití nástroje Vyčištění disku stále málo místa, je možné, že se vaše složka Temp rychle plní soubory aplikací (.appx), které používá Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="9d336-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="9d336-107">Tento problém vyřešíte resetováním Microsoft Store, vymazáním mezipaměti Microsoft Store a spuštěním poradce při potížích služby Windows Update.</span><span class="sxs-lookup"><span data-stu-id="9d336-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="9d336-108">Zavřete Microsoft Store předtím, než se pustíte do těchto kroků.</span><span class="sxs-lookup"><span data-stu-id="9d336-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="9d336-109">**Krok 1: Resetujte Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="9d336-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="9d336-110">**Poznámka** Tímto krokem dojde k trvalému smazání dat aplikace na zařízení, včetně vašich předvoleb a přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="9d336-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="9d336-111">Vyberte **Start** > **Nastavení** > **Aplikace** > **Aplikace a funkce**.</span><span class="sxs-lookup"><span data-stu-id="9d336-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="9d336-112">V seznamu aplikací najděte a vyberte Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="9d336-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="9d336-113">Vyberte **Upřesnit možnosti**.</span><span class="sxs-lookup"><span data-stu-id="9d336-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="9d336-114">Posuňte se dolů a vyberte **Resetovat** a pak **Potvrdit resetování**.</span><span class="sxs-lookup"><span data-stu-id="9d336-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="9d336-115">**Krok 2: Vymažte mezipaměť Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="9d336-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="9d336-116">Stisknutím klávesy s logem Windows + R otevřete dialogové okno Spustit.</span><span class="sxs-lookup"><span data-stu-id="9d336-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="9d336-117">Napište wsreset.exe a zvolte **OK**.</span><span class="sxs-lookup"><span data-stu-id="9d336-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="9d336-118">Otevře se prázdné okno příkazového řádku.</span><span class="sxs-lookup"><span data-stu-id="9d336-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="9d336-119">Po asi 10 sekundách se okno zavře a Microsoft Store se automaticky otevře.</span><span class="sxs-lookup"><span data-stu-id="9d336-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="9d336-120">**Krok 3: Resetujte službu Windows Update**</span><span class="sxs-lookup"><span data-stu-id="9d336-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="9d336-121">Vyberte **Start** > **Nastavení** > **Aktualizace a zabezpečení** > **Řešení potíží**.</span><span class="sxs-lookup"><span data-stu-id="9d336-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="9d336-122">Posuňte se dolů a ze seznamu vyberte **Služba Windows Update**, pak zvolte **Spustit poradce při potížích**.</span><span class="sxs-lookup"><span data-stu-id="9d336-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="9d336-123">Restartujte počítač a zkontrolujte, jestli pořád dochází k potížím.</span><span class="sxs-lookup"><span data-stu-id="9d336-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

