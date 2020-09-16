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
# <a name="startup-settings-in-windows-10"></a>Nastavení při spuštění ve Windows 10

**Změna aplikací spouštěných automaticky při spuštění**

1. Přejděte na [nastavení > aplikace > spuštění](ms-settings:startupapps?activationSource=GetHelp).

2. Ujistěte se, že **je zapnutá**jakákoli aplikace, kterou chcete spustit při spuštění.

**Přidání aplikace tak, aby se spouštěla automaticky při spuštění**

1. Klikněte nebo klepněte na **Spustit** a Najděte aplikaci, kterou chcete spustit při spuštění.

2. Klikněte pravým tlačítkem na aplikaci, klikněte na **Další**a potom klikněte na **Otevřít umístění souboru**. Otevře se místo, kde se zástupce aplikace uloží. Pokud není možnost Otevřít umístění souboru k dispozici, znamená to, že se aplikace nemůže spustit při spuštění.

3. V otevřeném umístění souboru stiskněte klávesu s **logem Windows + R**, zadejte **Shell: Startup**a klikněte na **OK**. Otevře se složka po spuštění.

4. Zkopírujte a vložte zástupce do aplikace z umístění souboru do složky po spuštění.

**Rozšířené možnosti spuštění (včetně nouzového režimu, nastavení UEFI a spuštění z jiného zařízení)**

1. Uložte svoji práci a zavřete všechny otevřené dokumenty, protože tento postup restartuje počítač.

2. Přejděte na [nastavení > aktualizace > & zabezpečení](ms-settings:recovery?activationSource=GetHelp).

3. V části **Rozšířené spuštění**klikněte na **restartovat**. 

4. Po restartování počítače na obrazovku zvolit možnost:

    - Pokud chcete počítač spustit ze zařízení, jako je USB disk, klikněte na **použít zařízení**.

    - Pokud chcete zadat nastavení UEFI (někdy nazývané nastavení systému BIOS), klikněte na **Poradce při potížích s > Upřesnit možnosti > nastavení firmwaru UEFI**. 

    - Pokud chcete přejít do nouzového režimu nebo změnit upřesňující nastavení spuštění, klikněte na **Poradce při potížích s > Upřesnit možnosti > nastavení spouštění**a pak klikněte na **restartovat**. Můžete být požádáni, abyste zadali [obnovovací klíč nástroje BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Po dalším restartování počítače klikněte na nastavení spouštění, které chcete použít.