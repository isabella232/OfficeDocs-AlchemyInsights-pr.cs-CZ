---
title: Ikona napájení nebo baterie chybí ve Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790541"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="8524d-102">Ikona napájení nebo baterie chybí ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="8524d-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="8524d-103">Pokud má zařízení s Windows 10 ikonu baterie (např. přenosný počítač, tablet nebo počítač připojený přes USB k UPS), obvykle se na hlavním panelu poblíž hodin zobrazí ikona napájení/baterie, například:</span><span class="sxs-lookup"><span data-stu-id="8524d-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikona baterie](media/battery-icon.png)

<span data-ttu-id="8524d-105">Pokud tuto ikonu nevidíte, může být skrytá:</span><span class="sxs-lookup"><span data-stu-id="8524d-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="8524d-106">Přejděte na **[Nastavení > Přizpůsobení > Hlavní panel](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="8524d-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="8524d-107">V oznamovací oblasti klikněte na **Vyberte, které ikony se zobrazí na hlavním panelu**.</span><span class="sxs-lookup"><span data-stu-id="8524d-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="8524d-108">Potom najděte položku **Napájení (Power)** v seznamu a přepněte nastavení na **Zapnuté**.</span><span class="sxs-lookup"><span data-stu-id="8524d-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Zobrazení ikony napájení na hlavním panelu](media/power-icon-on.png)

<span data-ttu-id="8524d-110">**Řešení potíží**</span><span class="sxs-lookup"><span data-stu-id="8524d-110">**Troubleshooting**</span></span>

<span data-ttu-id="8524d-111">Pokud jste postupovali podle výše uvedených pokynů a přepínač **Napájení (Power)** je zobrazený šedě nebo není viditelný, zadejte do vyhledávacího pole na hlavním panelu **správce zařízení** a potom v seznamu výsledků vyberte **Správce zařízení**.</span><span class="sxs-lookup"><span data-stu-id="8524d-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="8524d-112">V části **Baterie** klikněte pravým tlačítkem myši na ikonu baterie vašeho zařízení, klikněte na možnost **Vypnout** a potom na **Ano**.</span><span class="sxs-lookup"><span data-stu-id="8524d-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="8524d-113">Počkejte několik sekund a potom klikněte pravým tlačítkem myši na ikonu baterie a na **Zapnout**.</span><span class="sxs-lookup"><span data-stu-id="8524d-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="8524d-114">Pak restartujte zařízení.</span><span class="sxs-lookup"><span data-stu-id="8524d-114">Then restart your device.</span></span>

<span data-ttu-id="8524d-115">Pokud jste postupovali podle výše uvedených pokynů, ale ikona baterie se nezobrazuje na hlavním panelu, zadejte do vyhledávacího pole na hlavním panelu **správce úloh** a potom v seznamu výsledků klikněte na **Správce úloh**.</span><span class="sxs-lookup"><span data-stu-id="8524d-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="8524d-116">Na kartě **Procesy** klikněte v části **Název** pravým tlačítkem na **Explorer** a potom klikněte na **Restartovat**.</span><span class="sxs-lookup"><span data-stu-id="8524d-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
