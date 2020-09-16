---
title: Řešení problémů s Bluetooth ve Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730152"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="d80b7-102">Řešení problémů s Bluetooth ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="d80b7-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="d80b7-103">Pokud ikona Bluetooth chybí nebo ji Bluetooth nejde zapnout nebo vypnout, můžete spustit Poradce při potížích s Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="d80b7-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="d80b7-104">[Otevřete nastavení Poradce při potížích](ms-settings:troubleshoot), v části **Najít a opravit další problémy**klikněte na **Bluetooth** a pak klikněte na **spustit Poradce při potížích**.</span><span class="sxs-lookup"><span data-stu-id="d80b7-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="d80b7-105">Pokud ikonu Bluetooth nevidíte, zobrazí se ve Správci zařízení Bluetooth:</span><span class="sxs-lookup"><span data-stu-id="d80b7-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="d80b7-106">Ve Správci zařízení klikněte na **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="d80b7-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="d80b7-107">Stiskněte a podržte (nebo pravým tlačítkem myši) název adaptéru Bluetooth a klikněte na **odinstalovat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="d80b7-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="d80b7-108">Vypněte zařízení s Windows, počkejte pár sekund a pak ho znovu zapněte.</span><span class="sxs-lookup"><span data-stu-id="d80b7-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="d80b7-109">Systém Windows se pokusí ovladač přeinstalovat.</span><span class="sxs-lookup"><span data-stu-id="d80b7-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="d80b7-110">Pokud jste nedávno nainstalovali aktualizace Windows 10 nebo jste upgradovali na Windows 10, můžete zkontrolovat aktualizace ovladačů:</span><span class="sxs-lookup"><span data-stu-id="d80b7-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="d80b7-111">Ve Správci zařízení klikněte na **Bluetooth**a potom klikněte na název adaptéru Bluetooth (který by mohl zahrnovat slovo "Radio").</span><span class="sxs-lookup"><span data-stu-id="d80b7-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="d80b7-112">Stiskněte a podržte (nebo klikněte pravým tlačítkem myši) na adaptér Bluetooth a pak klikněte na **aktualizovat**  >  **hledání ovladače automaticky pro aktualizovaný software ovladače**.</span><span class="sxs-lookup"><span data-stu-id="d80b7-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="d80b7-113">Postupujte podle pokynů a potom klikněte na **Zavřít**.</span><span class="sxs-lookup"><span data-stu-id="d80b7-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="d80b7-114">Pokud systém Windows nenašel nový ovladač Bluetooth, navštivte web výrobce počítače a Stáhněte si nejnovější ovladač Bluetooth odtud.</span><span class="sxs-lookup"><span data-stu-id="d80b7-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="d80b7-115">Po stažení klikněte na **Aktualizovat ovladač**.  >  **Vyhledat na počítači ovladače**  >  **vyhledejte** umístění, kde jsou soubory ovladače uloženy > **OK**  >  **Next**a postupujte podle pokynů k instalaci.</span><span class="sxs-lookup"><span data-stu-id="d80b7-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="d80b7-116">Po instalaci aktualizovaného ovladače restartujte počítač a pak zkontrolujte, jestli je problém s připojením vyřešený.</span><span class="sxs-lookup"><span data-stu-id="d80b7-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="d80b7-117">Podrobnější informace o řešení problémů s Bluetooth najdete v článku úplné řešení [problémů s Bluetooth ve Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="d80b7-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
