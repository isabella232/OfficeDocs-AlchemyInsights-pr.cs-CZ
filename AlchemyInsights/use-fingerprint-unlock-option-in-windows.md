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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="1befa-102">Použití možnosti odemknutí otiskem prstu ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="1befa-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="1befa-103">**Povolit otisk prstu Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="1befa-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="1befa-104">Chcete-li odemknout Windows 10 pomocí otisku prstu, musíte nastavit otisk prstu Windows Hello přidáním (Přihlaste se systému Windows) aspoň jedním prstem.</span><span class="sxs-lookup"><span data-stu-id="1befa-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="1befa-105">Přejděte na **nastavení > účty > možnosti přihlášení** (nebo klikněte [sem](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="1befa-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="1befa-106">Budou dostupné možnosti přihlášení.</span><span class="sxs-lookup"><span data-stu-id="1befa-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="1befa-107">Příklad:</span><span class="sxs-lookup"><span data-stu-id="1befa-107">For example:</span></span>

    ![Možnosti přihlášení](media/sign-in-options.png)

2. <span data-ttu-id="1befa-109">Klikněte nebo klepněte na **otisk prstu Windows Hello**a pak klikněte na **nastavit**.</span><span class="sxs-lookup"><span data-stu-id="1befa-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="1befa-110">V okně nastavení Windows Hello klikněte na **Začínáme.**</span><span class="sxs-lookup"><span data-stu-id="1befa-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="1befa-111">Senzor otisků prstů se aktivuje a zobrazí se výzva k zadání prstu na senzor:</span><span class="sxs-lookup"><span data-stu-id="1befa-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor otisků prstů](media/fingerprint-sensor.png)

3. <span data-ttu-id="1befa-113">Postupujte podle pokynů, které vám požádají o opakované prohledání prstu.</span><span class="sxs-lookup"><span data-stu-id="1befa-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="1befa-114">Po dokončení budete mít možnost přidat další prsty, které můžete použít k přihlášení.</span><span class="sxs-lookup"><span data-stu-id="1befa-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="1befa-115">Při příštím přihlášení k Windows 10 budete mít k tomu k dispozici možnost použít váš otisk prstu.</span><span class="sxs-lookup"><span data-stu-id="1befa-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="1befa-116">**Otisk prstu Windows Hello není k dispozici jako možnost přihlášení**</span><span class="sxs-lookup"><span data-stu-id="1befa-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="1befa-117">Pokud se otisk prstu Windows Hello nezobrazuje jako možnost v **možnostech přihlášení**, znamená to, že se v systému Windows nezobrazuje žádné čtecí zařízení a skenery otisků prstů připojené k počítači</span><span class="sxs-lookup"><span data-stu-id="1befa-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="1befa-118">Řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="1befa-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="1befa-119">Na hlavním panelu vyberte tlačítko **Start** a vyhledejte **Správce zařízení**.</span><span class="sxs-lookup"><span data-stu-id="1befa-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="1befa-120">Kliknutím nebo klepnutím otevřete **Správce zařízení**.</span><span class="sxs-lookup"><span data-stu-id="1befa-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="1befa-121">Ve Správci zařízení rozbalte položku biometrické zařízení kliknutím na její dvojitou šipku.</span><span class="sxs-lookup"><span data-stu-id="1befa-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrické zařízení.](media/biometric-devices.png)

4. <span data-ttu-id="1befa-123">Váš otisk prstu by měl být uvedený jako biometrické zařízení, třeba na Synaptics WBDI Scanner:</span><span class="sxs-lookup"><span data-stu-id="1befa-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrické zařízení.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="1befa-125">Pokud váš otisk prstu není zobrazený a skener je integrovaný do počítače, přejděte na web výrobce počítače.</span><span class="sxs-lookup"><span data-stu-id="1befa-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="1befa-126">V části technická podpora pro váš model vašeho počítače vyhledejte ovladač pro skener s Windows 10, který můžete nainstalovat.</span><span class="sxs-lookup"><span data-stu-id="1befa-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="1befa-127">Pokud je skener oddělený od počítače (připojený přes USB), přejděte na web výrobce skeneru a vyhledejte a nainstalujte si software ovladače zařízení s Windows 10 pro model skeneru, který máte.</span><span class="sxs-lookup"><span data-stu-id="1befa-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
