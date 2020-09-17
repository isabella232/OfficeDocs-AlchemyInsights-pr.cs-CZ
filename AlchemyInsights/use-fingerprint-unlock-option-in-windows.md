---
title: Použití možnosti odemknutí otiskem prstu ve Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795237"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Použití možnosti odemknutí otiskem prstu ve Windows 10

**Povolit otisk prstu Windows Hello**

Chcete-li odemknout Windows 10 pomocí otisku prstu, musíte nastavit otisk prstu Windows Hello přidáním (Přihlaste se systému Windows) aspoň jedním prstem. 

1. Přejděte na **nastavení > účty > možnosti přihlášení** (nebo klikněte [sem](ms-settings:signinoptions?activationSource=GetHelp)). Budou dostupné možnosti přihlášení. Příklad:

    ![Možnosti přihlášení](media/sign-in-options.png)

2. Klikněte nebo klepněte na **otisk prstu Windows Hello**a pak klikněte na **nastavit**. V okně nastavení Windows Hello klikněte na **Začínáme.** Senzor otisků prstů se aktivuje a zobrazí se výzva k zadání prstu na senzor:

   ![Senzor otisků prstů](media/fingerprint-sensor.png)

3. Postupujte podle pokynů, které vám požádají o opakované prohledání prstu. Po dokončení budete mít možnost přidat další prsty, které můžete použít k přihlášení. Při příštím přihlášení k Windows 10 budete mít k tomu k dispozici možnost použít váš otisk prstu.

**Otisk prstu Windows Hello není k dispozici jako možnost přihlášení**

Pokud se otisk prstu Windows Hello nezobrazuje jako možnost v **možnostech přihlášení**, znamená to, že se v systému Windows nezobrazuje žádné čtecí zařízení a skenery otisků prstů připojené k počítači Řešení potíží: 

1. Na hlavním panelu vyberte tlačítko **Start** a vyhledejte **Správce zařízení**.

2. Kliknutím nebo klepnutím otevřete **Správce zařízení**.

3. Ve Správci zařízení rozbalte položku biometrické zařízení kliknutím na její dvojitou šipku.

   ![Biometrické zařízení.](media/biometric-devices.png)

4. Váš otisk prstu by měl být uvedený jako biometrické zařízení, třeba na Synaptics WBDI Scanner:

   ![Biometrické zařízení.](media/biometric-devices-expanded.png)

5. Pokud váš otisk prstu není zobrazený a skener je integrovaný do počítače, přejděte na web výrobce počítače. V části technická podpora pro váš model vašeho počítače vyhledejte ovladač pro skener s Windows 10, který můžete nainstalovat.

6. Pokud je skener oddělený od počítače (připojený přes USB), přejděte na web výrobce skeneru a vyhledejte a nainstalujte si software ovladače zařízení s Windows 10 pro model skeneru, který máte.
