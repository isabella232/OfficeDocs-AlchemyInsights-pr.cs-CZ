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
# <a name="startup-settings-in-windows-10"></a>Nastavení spouštění ve Windows 10

**Změna automaticky spouštěné aplikace při spuštění**

1. Přejděte na [Nastavení > aplikace > spuštění](ms-settings:startupapps?activationSource=GetHelp).

2. Ujistěte se, že je zapnutá jakákoli aplikace, kterou chcete spustit při **spuštění.**

**Přidání aplikace, která se má spouštět automaticky při spuštění**

1. Klikněte nebo klepněte **na Start** a najděte aplikaci, kterou chcete spustit při spuštění.

2. Klikněte pravým tlačítkem myši na aplikaci, klikněte **na Další** a potom klikněte na Otevřít **umístění souboru.** Tím se otevře umístění, kam se zástupce aplikace uloží. Pokud není možnost Pro otevření umístění souboru, znamená to, že aplikace nemůže běžet při spuštění.

3. S otevřeným umístěním souboru stiskněte klávesu **s logem Windows + R**, zadejte **shell:startup** a klikněte na **OK.** Tím se otevře složka Po spuštění.

4. Zkopírujte a vložte zástupce aplikace z umístění souboru do složky Po spuštění.

**Rozšířené možnosti spuštění (včetně nouzového režimu, nastavení UEFI a spouštění z jiného zařízení)**

1. Uložte si práci a zavřete všechny otevřené dokumenty, protože tento postup restartuje počítač.

2. Přejděte na [Nastavení > Aktualizace & zabezpečení > obnovení](ms-settings:recovery?activationSource=GetHelp).

3. V **části Advanced startup (Upřesnit** spuštění) klikněte na Restart now **(Restartovat).** 

4. Po restartování počítače na obrazovce Zvolit možnost:

    - Pokud chcete spustit systém ze zařízení, jako je usb disk, klikněte **na Použít zařízení.**

    - Pokud chcete zadat nastavení UEFI (někdy se tomu říká nastavení systému BIOS), klikněte na Poradce při potížích > Upřesnit možnosti > **nastavení firmwaru UEFI.** 

    - Pokud chcete vstoupit do nouzového režimu nebo změnit upřesňující nastavení spouštění, klikněte na > Upřesnit možnosti **> Nastavení spuštění** a potom klikněte na **Restartovat.** Může se zobrazit dotaz, jestli chcete zadat [obnovovací klíč nástroje BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Po opětovném restartování počítače klikněte na nastavení spouštění, které chcete použít.