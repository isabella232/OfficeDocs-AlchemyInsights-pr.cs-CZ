---
title: Řešení potíží se stávajícím monitorem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824572"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="03432-102">Poradce při potížích s existujícím monitorem</span><span class="sxs-lookup"><span data-stu-id="03432-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="03432-103">Vyzkoušejte tato řešení pro řešení potíží s monitorem.</span><span class="sxs-lookup"><span data-stu-id="03432-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="03432-104">**Aktualizace zobrazení monitoru:**</span><span class="sxs-lookup"><span data-stu-id="03432-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="03432-105">Stiskněte současně následující klávesy: Klávesa Windows + Ctrl + Shift + B. Tím se obnoví komunikace s ovladačem grafické karty.</span><span class="sxs-lookup"><span data-stu-id="03432-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="03432-106">Vaše monitory budou na okamžik blikat a po několika sekundách se vrátí.</span><span class="sxs-lookup"><span data-stu-id="03432-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="03432-107">**Poradce při potížích s hardwarem monitoru:**</span><span class="sxs-lookup"><span data-stu-id="03432-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="03432-108">Odpojte kabel připojující počítač k monitoru a znovu ho připojte.</span><span class="sxs-lookup"><span data-stu-id="03432-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="03432-109">Odpojte všechna zařízení, která nejsou nezbytná, od počítače (například adaptéry nebo doky).</span><span class="sxs-lookup"><span data-stu-id="03432-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="03432-110">**Pokud jste nedávno nainstalovali aktualizaci na počítači, můžete ovladač zobrazení vrátit zpět:**</span><span class="sxs-lookup"><span data-stu-id="03432-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="03432-111">Vyberte **Start,** zadejte **Správce zařízení** a ve **výsledcích** vyberte Správce zařízení.</span><span class="sxs-lookup"><span data-stu-id="03432-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="03432-112">Rozbalte **část Grafické adaptéry,** klikněte pravým tlačítkem myši na grafický adaptér a vyberte **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="03432-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="03432-113">Přejděte na kartu **Ovladač** a vyberte **Vrátit ovladač zpět.**</span><span class="sxs-lookup"><span data-stu-id="03432-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="03432-114">Poznámka: Pokud tato možnost není dostupná nebo  je šedě šedě, vyberte v následujících možnostech možnost Ne a přejděte k dalšímu kroku.</span><span class="sxs-lookup"><span data-stu-id="03432-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="03432-115">Možná budete muset restartovat počítač, než se tyto změny projeví.</span><span class="sxs-lookup"><span data-stu-id="03432-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="03432-116">**Odinstalace a přeinstalace ovladače zobrazení:**</span><span class="sxs-lookup"><span data-stu-id="03432-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="03432-117">Vyberte **Start,** zadejte **Správce zařízení** a ve **výsledcích** vyberte Správce zařízení.</span><span class="sxs-lookup"><span data-stu-id="03432-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="03432-118">Rozbalte **část Grafické adaptéry,** klikněte pravým tlačítkem myši na grafický adaptér a vyberte **Odinstalovat zařízení.**</span><span class="sxs-lookup"><span data-stu-id="03432-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="03432-119">Zaškrtněte políčko Vedle možnosti **Odstranit software ovladače pro toto zařízení a** vyberte **Odinstalovat.**</span><span class="sxs-lookup"><span data-stu-id="03432-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="03432-120">Poznámka: V této fázi se může zobrazit dotaz, jestli chcete restartovat počítač.</span><span class="sxs-lookup"><span data-stu-id="03432-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="03432-121">Před restartováním si nezapomeňte zapsat zbývající pokyny.</span><span class="sxs-lookup"><span data-stu-id="03432-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="03432-122">Znovu otevřete Správce zařízení.</span><span class="sxs-lookup"><span data-stu-id="03432-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="03432-123">Rozbalte **část Grafické adaptéry,** klikněte pravým tlačítkem myši na grafický adaptér a vyberte **Aktualizovat ovladač.**</span><span class="sxs-lookup"><span data-stu-id="03432-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="03432-124">Vyberte **Automaticky hledat aktualizační software ovladače** a postupujte podle pokynů k instalaci.</span><span class="sxs-lookup"><span data-stu-id="03432-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>