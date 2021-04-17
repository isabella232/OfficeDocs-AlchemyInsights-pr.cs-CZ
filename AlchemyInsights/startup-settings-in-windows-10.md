---
title: Nastavení spouštění ve Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828145"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="1018e-102">Nastavení spouštění ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="1018e-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="1018e-103">**Změna automaticky spouštěné aplikace při spuštění**</span><span class="sxs-lookup"><span data-stu-id="1018e-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="1018e-104">Přejděte na [Nastavení > aplikace > spuštění](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="1018e-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="1018e-105">Ujistěte se, že je zapnutá jakákoli aplikace, kterou chcete spustit při **spuštění.**</span><span class="sxs-lookup"><span data-stu-id="1018e-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="1018e-106">**Přidání aplikace, která se má spouštět automaticky při spuštění**</span><span class="sxs-lookup"><span data-stu-id="1018e-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="1018e-107">Klikněte nebo klepněte **na Start** a najděte aplikaci, kterou chcete spustit při spuštění.</span><span class="sxs-lookup"><span data-stu-id="1018e-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="1018e-108">Klikněte pravým tlačítkem myši na aplikaci, klikněte **na Další** a potom klikněte na Otevřít **umístění souboru.**</span><span class="sxs-lookup"><span data-stu-id="1018e-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="1018e-109">Tím se otevře umístění, kam se zástupce aplikace uloží.</span><span class="sxs-lookup"><span data-stu-id="1018e-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="1018e-110">Pokud není možnost Pro otevření umístění souboru, znamená to, že aplikace nemůže běžet při spuštění.</span><span class="sxs-lookup"><span data-stu-id="1018e-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="1018e-111">S otevřeným umístěním souboru stiskněte klávesu **s logem Windows + R**, zadejte **shell:startup** a klikněte na **OK.**</span><span class="sxs-lookup"><span data-stu-id="1018e-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="1018e-112">Tím se otevře složka Po spuštění.</span><span class="sxs-lookup"><span data-stu-id="1018e-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="1018e-113">Zkopírujte a vložte zástupce aplikace z umístění souboru do složky Po spuštění.</span><span class="sxs-lookup"><span data-stu-id="1018e-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="1018e-114">**Rozšířené možnosti spuštění (včetně nouzového režimu, nastavení UEFI a spouštění z jiného zařízení)**</span><span class="sxs-lookup"><span data-stu-id="1018e-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="1018e-115">Uložte si práci a zavřete všechny otevřené dokumenty, protože tento postup restartuje počítač.</span><span class="sxs-lookup"><span data-stu-id="1018e-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="1018e-116">Přejděte na [Nastavení > Aktualizace & zabezpečení > obnovení](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="1018e-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="1018e-117">V **části Advanced startup (Upřesnit** spuštění) klikněte na Restart now **(Restartovat).**</span><span class="sxs-lookup"><span data-stu-id="1018e-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="1018e-118">Po restartování počítače na obrazovce Zvolit možnost:</span><span class="sxs-lookup"><span data-stu-id="1018e-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="1018e-119">Pokud chcete spustit systém ze zařízení, jako je usb disk, klikněte **na Použít zařízení.**</span><span class="sxs-lookup"><span data-stu-id="1018e-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="1018e-120">Pokud chcete zadat nastavení UEFI (někdy se tomu říká nastavení systému BIOS), klikněte na Poradce při potížích > Upřesnit možnosti > **nastavení firmwaru UEFI.**</span><span class="sxs-lookup"><span data-stu-id="1018e-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="1018e-121">Pokud chcete vstoupit do nouzového režimu nebo změnit upřesňující nastavení spouštění, klikněte na > Upřesnit možnosti **> Nastavení spuštění** a potom klikněte na **Restartovat.**</span><span class="sxs-lookup"><span data-stu-id="1018e-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="1018e-122">Může se zobrazit dotaz, jestli chcete zadat [obnovovací klíč nástroje BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="1018e-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="1018e-123">Po opětovném restartování počítače klikněte na nastavení spouštění, které chcete použít.</span><span class="sxs-lookup"><span data-stu-id="1018e-123">After your PC restarts again, click the startup setting you want to use.</span></span>