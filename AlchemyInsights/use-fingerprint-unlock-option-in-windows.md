---
title: Použití možnosti odemknutí otisku prstu v Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971896"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Použití možnosti odemknutí otisku prstu v Windows 10

**Povolení Windows Hello otisku prstu**

Pokud chcete Windows 10 pomocí otisku Windows Hello prstu, musíte nastavit otisk prstu tak, že přidáte (Windows se naučíte rozpoznat) aspoň jedním prstem. 

1. Přejděte na **Nastavení > Účty > možnosti přihlášení** (nebo klikněte [sem).](ms-settings:signinoptions?activationSource=GetHelp) Zobrazí se dostupné možnosti přihlášení. Příklad:

    ![Možnosti přihlášení](media/sign-in-options.png)

2. Klikněte nebo klepněte **na Windows Hello Otisk prstu** a potom klikněte na **Nastavit.** V okně Windows Hello nastavení klikněte na **Začínáme.** Senzor otisku prstu se aktivuje a zobrazí se dotaz, jestli na senzor položíte prst:

   ![Senzor otisků prstů.](media/fingerprint-sensor.png)

3. Postupujte podle pokynů, které vás budou žádat, abyste prst opakovaně naskenoval. Po dokončení budete mít možnost přidat další prsty, které budete chtít použít pro přihlášení. Až se příště přihlásíte k Windows 10, budete k tomu mít možnost použít otisk prstu.

**Windows Hello Otisk prstu není k dispozici jako možnost přihlášení**

Pokud se v možnostech přihlášení nezobrazí možnost Otisk prstu **,** znamená to, že Windows o žádné čtečce otisků prstů nebo skeneru připojeném k počítači nebo o tom, že zásady systému brání jejímu použití (pokud například váš počítač spravuje vaše pracoviště). Windows Hello Řešení potíží: 

1. Na hlavním panelu vyberte tlačítko **Start** a vyhledejte **Správce zařízení.**

2. Kliknutím nebo klepnutím otevřete **Správce zařízení**.

3. Ve Správci zařízení rozbalte biometrická zařízení kliknutím na jeho chevron.

   ![Biometrická zařízení.](media/biometric-devices.png)

4. Skener otisků prstů by měl být uvedený jako biometrické zařízení, například skener Synaptics WBDI:

   ![Biometrická zařízení.](media/biometric-devices-expanded.png)

5. Pokud se čtečka otisků prstů nezobrazí a skener je integrovaný do počítače, přejděte na web výrobce počítače. V části technické podpory pro váš model počítače vyhledejte ovladač Windows 10 skeneru, který můžete nainstalovat.

6. Pokud je skener oddělený od počítače (připojeného přes USB), přejděte na web výrobce skeneru a vyhledejte Windows 10 nainstalujte software ovladače zařízení pro model skeneru, který máte.
