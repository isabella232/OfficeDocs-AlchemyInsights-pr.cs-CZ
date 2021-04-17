---
title: Řešení potíží se zvukem ve Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833284"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="0204e-102">Řešení potíží se zvukem ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="0204e-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="0204e-103">**Spuštění poradce při potížích se zvukem**</span><span class="sxs-lookup"><span data-stu-id="0204e-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="0204e-104">Otevřete nastavení [Poradce při potížích](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="0204e-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="0204e-105">Vyberte **Přehrát**  >  **zvuk: Spusťte poradce při potížích**.</span><span class="sxs-lookup"><span data-stu-id="0204e-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="0204e-106">**Nastavení výchozího zařízení**</span><span class="sxs-lookup"><span data-stu-id="0204e-106">**Set the default device**</span></span>

<span data-ttu-id="0204e-107">Pokud se připojujete ke zvukovému zařízení pomocí USB nebo HDMI, budete možná muset toto zařízení nastavit jako výchozí:</span><span class="sxs-lookup"><span data-stu-id="0204e-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="0204e-108">Otevřete **Spustit** zvuk a v seznamu výsledků vyberte Zvuk nebo Změnit systémové  >  zvuky.  </span><span class="sxs-lookup"><span data-stu-id="0204e-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="0204e-109">Na kartě **Přehrávání** vyberte zařízení, vyberte **Nastavit výchozí** a pak vyberte **OK.**</span><span class="sxs-lookup"><span data-stu-id="0204e-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="0204e-110">**Kontrola kabelů, hlasitosti, reproduktorů a sluchátek**</span><span class="sxs-lookup"><span data-stu-id="0204e-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="0204e-111">Zkontrolujte, jestli nejsou kabely reproduktoru a sluchátek připojené ke správnému konektoru, a zkontrolujte, jestli jsou připojené ke správnému konektoru.</span><span class="sxs-lookup"><span data-stu-id="0204e-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="0204e-112">Zkontrolujte úroveň napájení a hlasitosti a zkuste všechny ovládací prvky hlasitosti zesílit.</span><span class="sxs-lookup"><span data-stu-id="0204e-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="0204e-113">Některé reproduktory a aplikace mají vlastní ovládací prvky hlasitosti. Možná je budete muset všechny zkontrolovat, abyste měli jistotu, že jsou na správných úrovních.</span><span class="sxs-lookup"><span data-stu-id="0204e-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="0204e-114">Zkuste se připojit pomocí jiného portu USB.</span><span class="sxs-lookup"><span data-stu-id="0204e-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="0204e-115">**Poznámka:** Nezapomeňte, že reproduktory nemusí při připojení sluchátek fungovat.</span><span class="sxs-lookup"><span data-stu-id="0204e-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="0204e-116">**Kontrola Správce zařízení**</span><span class="sxs-lookup"><span data-stu-id="0204e-116">**Check Device Manager**</span></span>

<span data-ttu-id="0204e-117">Abyste měli jistotu, že jsou ovladače aktuální:</span><span class="sxs-lookup"><span data-stu-id="0204e-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="0204e-118">Vyberte **Start,** zadejte **Správce zařízení** a pak ze seznamu výsledků vyberte Správce zařízení. </span><span class="sxs-lookup"><span data-stu-id="0204e-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="0204e-119">V **části Ovladače zvuku, videa** a her vyberte zvukovou  kartu, otevřete ji, vyberte kartu Ovladač a vyberte **Aktualizovat ovladač**.</span><span class="sxs-lookup"><span data-stu-id="0204e-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="0204e-120">**Poznámka:** Pokud Systém Windows nenajde nový ovladač, vyhledejte ho na webu výrobce zařízení a postupujte podle jeho pokynů.</span><span class="sxs-lookup"><span data-stu-id="0204e-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="0204e-121">**Přeinstalace ovladače**</span><span class="sxs-lookup"><span data-stu-id="0204e-121">**Reinstall the driver**</span></span>

<span data-ttu-id="0204e-122">Pokud nemůžete aktualizovat přes Správce zařízení nebo najít nový ovladač na webu výrobce, zkuste tento postup:</span><span class="sxs-lookup"><span data-stu-id="0204e-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="0204e-123">Ve Správci zařízení klikněte pravým tlačítkem myši (nebo stiskněte a podržte) ovladač zvuku a vyberte **Odinstalovat.**</span><span class="sxs-lookup"><span data-stu-id="0204e-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="0204e-124">Restartujte zařízení a Windows se pokusí ovladač přeinstalovat.</span><span class="sxs-lookup"><span data-stu-id="0204e-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="0204e-125">Pokud přeinstalace ovladače nefunguje, zkuste použít obecný ovladač zvuku, který je součástí Windows.</span><span class="sxs-lookup"><span data-stu-id="0204e-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="0204e-126">Ve Správci zařízení klikněte pravým tlačítkem myši (nebo stiskněte a podržte) ovladač zvuku > Aktualizovat software ovladače Projděte si software ovladače Na počítači si vyberu ze seznamu ovladačů zařízení na mém počítači , vyberte Zvukové zařízení s vysokým rozlišením , vyberte Další a nainstalujte ho podle  >    >  pokynů.  </span><span class="sxs-lookup"><span data-stu-id="0204e-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
