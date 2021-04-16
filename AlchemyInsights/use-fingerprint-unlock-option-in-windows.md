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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="87614-102">Použití možnosti odemknutí otisku prstu ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="87614-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="87614-103">**Povolení otisku prstu ve Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="87614-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="87614-104">Pokud chcete odemknout Windows 10 pomocí otisku prstu, musíte nastavit Windows Hello Fingerprint přidáním (aby se Systém Windows naučil rozpoznávat) aspoň jedním prstem.</span><span class="sxs-lookup"><span data-stu-id="87614-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="87614-105">Přejděte na **Nastavení > Účty > možnosti přihlášení** (nebo klikněte [sem).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="87614-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="87614-106">Zobrazí se dostupné možnosti přihlášení.</span><span class="sxs-lookup"><span data-stu-id="87614-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="87614-107">Příklad:</span><span class="sxs-lookup"><span data-stu-id="87614-107">For example:</span></span>

    ![Možnosti přihlášení](media/sign-in-options.png)

2. <span data-ttu-id="87614-109">Klikněte nebo klepněte na **Windows Hello Fingerprint** a potom na **Nastavit.**</span><span class="sxs-lookup"><span data-stu-id="87614-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="87614-110">V okně nastavení Windows Hello klikněte na **Začínáme.**</span><span class="sxs-lookup"><span data-stu-id="87614-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="87614-111">Senzor otisku prstu se aktivuje a zobrazí se dotaz, jestli na senzor položíte prst:</span><span class="sxs-lookup"><span data-stu-id="87614-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor otisků prstů.](media/fingerprint-sensor.png)

3. <span data-ttu-id="87614-113">Postupujte podle pokynů, které vás budou žádat, abyste prst opakovaně naskenoval.</span><span class="sxs-lookup"><span data-stu-id="87614-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="87614-114">Po dokončení budete mít možnost přidat další prsty, které budete chtít použít pro přihlášení.</span><span class="sxs-lookup"><span data-stu-id="87614-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="87614-115">Až se příště přihlásíte k Windows 10, budete k tomu mít možnost použít otisk prstu.</span><span class="sxs-lookup"><span data-stu-id="87614-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="87614-116">**Otisk prstu Windows Hello není k dispozici jako možnost přihlášení**</span><span class="sxs-lookup"><span data-stu-id="87614-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="87614-117">Pokud se v možnostech přihlášení nezobrazí otisk prstu Windows Hello **,** znamená to, že Windows o žádné čtečce otisků prstů nebo skeneru připojeném k počítači ani o tom, že zásady systému brání jeho použití (pokud například váš počítač spravuje vaše pracoviště).</span><span class="sxs-lookup"><span data-stu-id="87614-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="87614-118">Řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="87614-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="87614-119">Na hlavním panelu vyberte tlačítko **Start** a vyhledejte **Správce zařízení.**</span><span class="sxs-lookup"><span data-stu-id="87614-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="87614-120">Kliknutím nebo klepnutím otevřete **Správce zařízení**.</span><span class="sxs-lookup"><span data-stu-id="87614-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="87614-121">Ve Správci zařízení rozbalte biometrická zařízení kliknutím na jeho chevron.</span><span class="sxs-lookup"><span data-stu-id="87614-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrická zařízení.](media/biometric-devices.png)

4. <span data-ttu-id="87614-123">Skener otisků prstů by měl být uvedený jako biometrické zařízení, například skener Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="87614-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrická zařízení.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="87614-125">Pokud se čtečka otisků prstů nezobrazí a skener je integrovaný do počítače, přejděte na web výrobce počítače.</span><span class="sxs-lookup"><span data-stu-id="87614-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="87614-126">V části technické podpory vašeho modelu počítače vyhledejte ovladač Windows 10 pro skener, který můžete nainstalovat.</span><span class="sxs-lookup"><span data-stu-id="87614-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="87614-127">Pokud je skener oddělený od počítače (připojeného přes USB), přejděte na web výrobce skeneru a vyhledejte a nainstalujte software ovladače zařízení s Windows 10 pro model skeneru, který máte.</span><span class="sxs-lookup"><span data-stu-id="87614-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
