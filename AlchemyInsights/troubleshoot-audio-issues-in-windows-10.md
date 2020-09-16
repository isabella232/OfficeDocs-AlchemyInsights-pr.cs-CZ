---
title: Poradce při potížích se zvukem ve Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750300"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="5dbc3-102">Řešení problémů se zvukem ve Windows 10</span><span class="sxs-lookup"><span data-stu-id="5dbc3-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="5dbc3-103">**Spuštění Poradce při potížích se zvukem**</span><span class="sxs-lookup"><span data-stu-id="5dbc3-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="5dbc3-104">Otevřete [nastavení Poradce při potížích](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="5dbc3-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="5dbc3-105">Vyberte **přehrávat zvuk**  >  **Spusťte Poradce při potížích**.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="5dbc3-106">**Nastavení výchozího zařízení**</span><span class="sxs-lookup"><span data-stu-id="5dbc3-106">**Set the default device**</span></span>

<span data-ttu-id="5dbc3-107">Pokud se připojujete ke zvukovému zařízení přes USB nebo HDMI, možná budete muset nastavit toto zařízení jako výchozí:</span><span class="sxs-lookup"><span data-stu-id="5dbc3-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="5dbc3-108">Otevřete **Start**  >  **zvuk**spuštění a v seznamu výsledků vyberte **zvuk** nebo **změnit systémové zvuky** .</span><span class="sxs-lookup"><span data-stu-id="5dbc3-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="5dbc3-109">Na kartě **přehrávání** vyberte zařízení, vyberte **nastavit výchozí**a pak vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="5dbc3-110">**Kontrola kabelů, hlasitosti, reproduktorů a sluchátek**</span><span class="sxs-lookup"><span data-stu-id="5dbc3-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="5dbc3-111">Zkontrolujte připojení reproduktorů a sluchátek, abyste mohli ztratit kabely, a ujistěte se, že jsou připojené ke správné zásuvce.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="5dbc3-112">Zkontrolujte úrovně napájení a hlasitosti a zkuste nastavit všechny ovladače hlasitosti.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="5dbc3-113">Některé reproduktory a aplikace mají vlastní ovládání hlasitosti. je možné, že všechny zkontrolujete, jestli jsou na správných úrovních.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="5dbc3-114">Zkuste se připojit pomocí jiného portu USB.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="5dbc3-115">**Poznámka**: Pokud jsou sluchátka zapojená, nemusí se vaše reproduktory správně pracovat.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="5dbc3-116">**Kontrola Správce zařízení**</span><span class="sxs-lookup"><span data-stu-id="5dbc3-116">**Check Device Manager**</span></span>

<span data-ttu-id="5dbc3-117">Jestli máte aktuální ovladače, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="5dbc3-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="5dbc3-118">Vyberte **Start**, zadejte **Správce zařízení**a potom v seznamu výsledků vyberte **Správce zařízení** .</span><span class="sxs-lookup"><span data-stu-id="5dbc3-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="5dbc3-119">V části ovladače **zvuku, videa a herních zařízení**vyberte zvukovou kartu, otevřete ji, vyberte kartu **ovladač** a vyberte **Aktualizovat ovladač**.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="5dbc3-120">**Poznámka**: Pokud systém Windows nenašel nový ovladač, hledejte ho na webu výrobce zařízení a postupujte podle pokynů.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="5dbc3-121">**Přeinstalace ovladače**</span><span class="sxs-lookup"><span data-stu-id="5dbc3-121">**Reinstall the driver**</span></span>

<span data-ttu-id="5dbc3-122">Pokud nemůžete provést aktualizaci prostřednictvím Správce zařízení nebo najít nový ovladač na webu výrobce, zkuste tento postup:</span><span class="sxs-lookup"><span data-stu-id="5dbc3-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="5dbc3-123">Ve Správci zařízení klikněte pravým tlačítkem (nebo stiskněte a podržte) ovladač zvuku a vyberte **odinstalovat**.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="5dbc3-124">Restartujte zařízení a Windows se pokusí ovladač přeinstalovat.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="5dbc3-125">Pokud přeinstalace ovladače nefunguje, zkuste použít obecný ovladač zvuku, který je součástí Windows.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="5dbc3-126">Ve Správci zařízení klikněte pravým tlačítkem (nebo stiskněte a podržte) svého ovladače zvuku > **aktualizovat software**ovladače  >  **Procházet můj počítač pro software ovladače**  >  : vybrat**ze seznamu ovladačů zařízení na mém počítači**vyberte **zvukové zařízení s vysokým rozlišením**, vyberte **Další**a postupujte podle pokynů k instalaci.</span><span class="sxs-lookup"><span data-stu-id="5dbc3-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
