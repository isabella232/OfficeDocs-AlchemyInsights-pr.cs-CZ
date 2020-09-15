---
title: Řešení potíží s existujícím monitorem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690704"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="d9126-102">Řešení potíží s existujícím monitorem</span><span class="sxs-lookup"><span data-stu-id="d9126-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="d9126-103">Pokud chcete vyřešit problém s monitorem, vyzkoušejte tato řešení.</span><span class="sxs-lookup"><span data-stu-id="d9126-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="d9126-104">**Aktualizace zobrazení monitoru:**</span><span class="sxs-lookup"><span data-stu-id="d9126-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="d9126-105">Současně stiskněte tyto klávesy: Klávesa Windows + CTRL + SHIFT + B. Touto akcí obnovíte komunikaci s grafickým ovladačem.</span><span class="sxs-lookup"><span data-stu-id="d9126-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="d9126-106">Monitory se budou za chvíli blikat a po několika sekundách se zase odeberou.</span><span class="sxs-lookup"><span data-stu-id="d9126-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="d9126-107">**Řešení potíží s hardwarem monitoru:**</span><span class="sxs-lookup"><span data-stu-id="d9126-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="d9126-108">Odpojte kabel spojující počítač s monitorem a zapojte ho zpátky.</span><span class="sxs-lookup"><span data-stu-id="d9126-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="d9126-109">Odpojte všechna nepotřebná zařízení z počítače (například z adaptérů nebo docků).</span><span class="sxs-lookup"><span data-stu-id="d9126-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="d9126-110">**Pokud jste si nedávno nainstalovali aktualizaci na počítač, můžete si vrátit zpátky svůj ovladač zobrazení:**</span><span class="sxs-lookup"><span data-stu-id="d9126-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="d9126-111">Vyberte **Start**, zadejte **Správce zařízení**a z výsledků vyberte **Správce zařízení** .</span><span class="sxs-lookup"><span data-stu-id="d9126-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d9126-112">Rozbalte oddíl Display Adapters ( **grafické adaptéry** ), klikněte pravým tlačítkem myši na grafický adaptér ANDS vyberte **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="d9126-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="d9126-113">Přejděte na kartu **ovladač** a vyberte **vrátit změny ovladače**.</span><span class="sxs-lookup"><span data-stu-id="d9126-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="d9126-114">Poznámka: Pokud tato možnost není dostupná nebo je zobrazená šedě, vyberte v možnostech níže možnost **ne** a přejděte tak k dalšímu kroku.</span><span class="sxs-lookup"><span data-stu-id="d9126-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="d9126-115">Aby se změny projevily, může být potřeba restartovat počítač.</span><span class="sxs-lookup"><span data-stu-id="d9126-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="d9126-116">**Odinstalace a přeinstalace ovladače zobrazení:**</span><span class="sxs-lookup"><span data-stu-id="d9126-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="d9126-117">Vyberte **Start**, zadejte **Správce zařízení**a z výsledků vyberte **Správce zařízení** .</span><span class="sxs-lookup"><span data-stu-id="d9126-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d9126-118">Rozbalte oddíl Display Adapters ( **grafické adaptéry** ), klikněte pravým tlačítkem myši na grafický adaptér ANDS vyberte **odinstalovat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="d9126-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="d9126-119">Zaškrtněte políčko vedle **Odstranit software ovladače tohoto zařízení** a vyberte **odinstalovat**.</span><span class="sxs-lookup"><span data-stu-id="d9126-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="d9126-120">Poznámka: můžete být požádáni o restartování počítače v této fázi.</span><span class="sxs-lookup"><span data-stu-id="d9126-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="d9126-121">Než začnete, zapište si zbývající pokyny.</span><span class="sxs-lookup"><span data-stu-id="d9126-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="d9126-122">Spusťte znovu Správce zařízení.</span><span class="sxs-lookup"><span data-stu-id="d9126-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="d9126-123">Rozbalte oddíl Display Adapters ( **grafické adaptéry** ), klikněte pravým tlačítkem na grafický adaptér a vyberte **Aktualizovat ovladač**.</span><span class="sxs-lookup"><span data-stu-id="d9126-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="d9126-124">**Pro aktualizaci softwaru ovladače vyberte Hledat automaticky** a postupujte podle pokynů k instalaci.</span><span class="sxs-lookup"><span data-stu-id="d9126-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>