---
title: Použití možnosti odemknutí otisku prstu ve Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796670"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Použití možnosti odemknutí otisku prstu ve Windows 10

**Povolení otisku prstu ve Windows Hello**

Pokud chcete odemknout Windows 10 pomocí otisku prstu, musíte nastavit Windows Hello Fingerprint přidáním (aby se Systém Windows naučil rozpoznávat) aspoň jedním prstem. 

1. Přejděte na **Nastavení > Účty > možnosti přihlášení** (nebo klikněte [sem).](ms-settings:signinoptions?activationSource=GetHelp) Zobrazí se dostupné možnosti přihlášení. Příklad:

    ![Možnosti přihlášení](media/sign-in-options.png)

2. Klikněte nebo klepněte na **Windows Hello Fingerprint** a potom na **Nastavit.** V okně nastavení Windows Hello klikněte na **Začínáme.** Senzor otisku prstu se aktivuje a zobrazí se dotaz, jestli na senzor položíte prst:

   ![Senzor otisků prstů.](media/fingerprint-sensor.png)

3. Postupujte podle pokynů, které vás budou žádat, abyste prst opakovaně naskenoval. Po dokončení budete mít možnost přidat další prsty, které budete chtít použít pro přihlášení. Až se příště přihlásíte k Windows 10, budete k tomu mít možnost použít otisk prstu.

**Otisk prstu Windows Hello není k dispozici jako možnost přihlášení**

Pokud se v možnostech přihlášení nezobrazí otisk prstu Windows Hello **,** znamená to, že Windows o žádné čtečce otisků prstů nebo skeneru připojeném k počítači ani o tom, že zásady systému brání jeho použití (pokud například váš počítač spravuje vaše pracoviště). Řešení potíží: 

1. Na hlavním panelu vyberte tlačítko **Start** a vyhledejte **Správce zařízení.**

2. Kliknutím nebo klepnutím otevřete **Správce zařízení**.

3. Ve Správci zařízení rozbalte biometrická zařízení kliknutím na jeho chevron.

   ![Biometrická zařízení.](media/biometric-devices.png)

4. Skener otisků prstů by měl být uvedený jako biometrické zařízení, například skener Synaptics WBDI:

   ![Biometrická zařízení.](media/biometric-devices-expanded.png)

5. Pokud se čtečka otisků prstů nezobrazí a skener je integrovaný do počítače, přejděte na web výrobce počítače. V části technické podpory vašeho modelu počítače vyhledejte ovladač Windows 10 pro skener, který můžete nainstalovat.

6. Pokud je skener oddělený od počítače (připojeného přes USB), přejděte na web výrobce skeneru a vyhledejte a nainstalujte software ovladače zařízení s Windows 10 pro model skeneru, který máte.
