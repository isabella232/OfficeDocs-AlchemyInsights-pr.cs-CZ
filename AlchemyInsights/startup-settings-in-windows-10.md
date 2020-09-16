---
title: Nastavení při spuštění ve Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751128"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="c20d8-102">Nastavení při spuštění ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="c20d8-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="c20d8-103">**Změna aplikací spouštěných automaticky při spuštění**</span><span class="sxs-lookup"><span data-stu-id="c20d8-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="c20d8-104">Přejděte na [nastavení > aplikace > spuštění](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="c20d8-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="c20d8-105">Ujistěte se, že **je zapnutá**jakákoli aplikace, kterou chcete spustit při spuštění.</span><span class="sxs-lookup"><span data-stu-id="c20d8-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="c20d8-106">**Přidání aplikace tak, aby se spouštěla automaticky při spuštění**</span><span class="sxs-lookup"><span data-stu-id="c20d8-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="c20d8-107">Klikněte nebo klepněte na **Spustit** a Najděte aplikaci, kterou chcete spustit při spuštění.</span><span class="sxs-lookup"><span data-stu-id="c20d8-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="c20d8-108">Klikněte pravým tlačítkem na aplikaci, klikněte na **Další**a potom klikněte na **Otevřít umístění souboru**.</span><span class="sxs-lookup"><span data-stu-id="c20d8-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="c20d8-109">Otevře se místo, kde se zástupce aplikace uloží.</span><span class="sxs-lookup"><span data-stu-id="c20d8-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="c20d8-110">Pokud není možnost Otevřít umístění souboru k dispozici, znamená to, že se aplikace nemůže spustit při spuštění.</span><span class="sxs-lookup"><span data-stu-id="c20d8-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="c20d8-111">V otevřeném umístění souboru stiskněte klávesu s **logem Windows + R**, zadejte **Shell: Startup**a klikněte na **OK**.</span><span class="sxs-lookup"><span data-stu-id="c20d8-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="c20d8-112">Otevře se složka po spuštění.</span><span class="sxs-lookup"><span data-stu-id="c20d8-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="c20d8-113">Zkopírujte a vložte zástupce do aplikace z umístění souboru do složky po spuštění.</span><span class="sxs-lookup"><span data-stu-id="c20d8-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="c20d8-114">**Rozšířené možnosti spuštění (včetně nouzového režimu, nastavení UEFI a spuštění z jiného zařízení)**</span><span class="sxs-lookup"><span data-stu-id="c20d8-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="c20d8-115">Uložte svoji práci a zavřete všechny otevřené dokumenty, protože tento postup restartuje počítač.</span><span class="sxs-lookup"><span data-stu-id="c20d8-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="c20d8-116">Přejděte na [nastavení > aktualizace > & zabezpečení](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="c20d8-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="c20d8-117">V části **Rozšířené spuštění**klikněte na **restartovat**.</span><span class="sxs-lookup"><span data-stu-id="c20d8-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="c20d8-118">Po restartování počítače na obrazovku zvolit možnost:</span><span class="sxs-lookup"><span data-stu-id="c20d8-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="c20d8-119">Pokud chcete počítač spustit ze zařízení, jako je USB disk, klikněte na **použít zařízení**.</span><span class="sxs-lookup"><span data-stu-id="c20d8-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="c20d8-120">Pokud chcete zadat nastavení UEFI (někdy nazývané nastavení systému BIOS), klikněte na **Poradce při potížích s > Upřesnit možnosti > nastavení firmwaru UEFI**.</span><span class="sxs-lookup"><span data-stu-id="c20d8-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="c20d8-121">Pokud chcete přejít do nouzového režimu nebo změnit upřesňující nastavení spuštění, klikněte na **Poradce při potížích s > Upřesnit možnosti > nastavení spouštění**a pak klikněte na **restartovat**.</span><span class="sxs-lookup"><span data-stu-id="c20d8-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="c20d8-122">Můžete být požádáni, abyste zadali [obnovovací klíč nástroje BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="c20d8-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="c20d8-123">Po dalším restartování počítače klikněte na nastavení spouštění, které chcete použít.</span><span class="sxs-lookup"><span data-stu-id="c20d8-123">After your PC restarts again, click the startup setting you want to use.</span></span>