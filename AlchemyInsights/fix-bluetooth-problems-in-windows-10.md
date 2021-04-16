---
title: Řešení problémů s Bluetooth ve Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812925"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="8efaa-102">Řešení problémů s Bluetooth ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="8efaa-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="8efaa-103">Pokud ikona Bluetooth chybí nebo bluetooth nelze zapnout nebo vypnout, můžete spustit Poradce při potížích s Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8efaa-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="8efaa-104">[Otevřete nastavení poradce při potížích,](ms-settings:troubleshoot) **klikněte na Bluetooth** v části Najít a opravit další **problémy** a klikněte na Spustit poradce **při potížích.**</span><span class="sxs-lookup"><span data-stu-id="8efaa-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="8efaa-105">Pokud ikonu Bluetooth nevidíte, ale Bluetooth se zobrazí ve Správci zařízení:</span><span class="sxs-lookup"><span data-stu-id="8efaa-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="8efaa-106">Ve Správci zařízení klikněte na **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="8efaa-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="8efaa-107">Stiskněte a podržte název adaptéru Bluetooth (nebo na něj klikněte pravým tlačítkem) a klikněte na **Odinstalovat zařízení.**</span><span class="sxs-lookup"><span data-stu-id="8efaa-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="8efaa-108">Vypněte zařízení s Windows, počkejte několik sekund a pak ho znovu zapněte.</span><span class="sxs-lookup"><span data-stu-id="8efaa-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="8efaa-109">Systém Windows se pokusí ovladač přeinstalovat.</span><span class="sxs-lookup"><span data-stu-id="8efaa-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="8efaa-110">Pokud jste nedávno nainstalovali aktualizace Windows 10 nebo upgradovali na Windows 10, možná budete chtít vyhledat aktualizace ovladačů:</span><span class="sxs-lookup"><span data-stu-id="8efaa-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="8efaa-111">Ve Správci zařízení klikněte na **Bluetooth** a potom klikněte na název adaptéru Bluetooth (který může obsahovat slovo "radio").</span><span class="sxs-lookup"><span data-stu-id="8efaa-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="8efaa-112">Stiskněte a podržte adaptér Bluetooth (nebo na něj klikněte pravým tlačítkem) a potom klikněte na Aktualizovat ovladač a vyhledejte aktualizovaný  >  **software ovladače automaticky.**</span><span class="sxs-lookup"><span data-stu-id="8efaa-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="8efaa-113">Postupujte podle pokynů a potom klikněte na **Zavřít.**</span><span class="sxs-lookup"><span data-stu-id="8efaa-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="8efaa-114">Pokud Systém Windows nemůže najít nový ovladač Bluetooth, navštivte web výrobce počítače a stáhněte si odtud nejnovější ovladač Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8efaa-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="8efaa-115">Po stažení klikněte na Aktualizovat ovladač Vyhledejte v počítači software ovladače Vyhledejte umístění, kde jsou soubory ovladačů  >    >   uložené, > **OK** Další a postupujte podle pokynů  >  k instalaci.</span><span class="sxs-lookup"><span data-stu-id="8efaa-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="8efaa-116">Po instalaci aktualizovaného ovladače restartujte počítač a zkontrolujte, jestli se tím problém s připojením opravuje.</span><span class="sxs-lookup"><span data-stu-id="8efaa-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="8efaa-117">Další informace o řešení potíží s Bluetooth najdete v úplném článku Řešení problémů [s Bluetooth ve Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="8efaa-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
