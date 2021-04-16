---
title: Soubor otevřený jen pro čtení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813177"
---
# <a name="file-open-read-only"></a><span data-ttu-id="ffc8c-102">Soubor otevřený jen pro čtení</span><span class="sxs-lookup"><span data-stu-id="ffc8c-102">File open read-only</span></span>

<span data-ttu-id="ffc8c-103">Možná zjistíte, že při otevírání souborů se otevřou jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="ffc8c-104">V některých případech je to kvůli přidanému zabezpečení, například když otevíráte soubory z internetu, a někdy to může být kvůli nastavení, které se může změnit.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="ffc8c-105">Tady jsou některé scénáře, kdy se soubor otevře jen pro čtení, a některé kroky, které můžete udělat, abyste ho změnili.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="ffc8c-106">**Antivirová ochrana způsobuje, že se otevřou jen pro čtení.**</span><span class="sxs-lookup"><span data-stu-id="ffc8c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="ffc8c-107">Některé antivirové programy vás mohou chránit před potenciálně nebezpečnými soubory tak, že je otevřete jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="ffc8c-108">Možná budete muset zkontrolovat poskytovatele antivirového softwaru, abyste se dozvěděli, jak tato nastavení upravit.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="ffc8c-109">BitDefender má například obsah při přidávání vyloučení aplikací tady: Jak přidat vyloučení aplikací nebo procesů v Centru řízení [bitdefenderu](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="ffc8c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="ffc8c-110">**Jsou vlastnosti souboru nastavené jen pro čtení?**</span><span class="sxs-lookup"><span data-stu-id="ffc8c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="ffc8c-111">Vlastnosti souboru můžete zkontrolovat tak, že na něj kliknete pravým tlačítkem a zvolíte Vlastnosti.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="ffc8c-112">Pokud je atribut jen pro čtení zaškrtnut, můžete ho zrušit a kliknout na OK.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="ffc8c-113">**Obsah je v chráněném zobrazení.**</span><span class="sxs-lookup"><span data-stu-id="ffc8c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="ffc8c-114">Soubory z internetu a z jiných potenciálně nebezpečných míst mohou obsahovat viry, červy nebo jiné druhy malwaru, které mohou poškodit váš počítač.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="ffc8c-115">To se často také používá u e-mailových příloh nebo souborů, které jste stáhli.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="ffc8c-116">K ochraně počítače se soubory z těchto potenciálně nebezpečných umístění otevře v chráněném zobrazení.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="ffc8c-117">Pomocí chráněného zobrazení si můžete přečíst soubor a zobrazit jeho obsah a zároveň snížit rizika.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="ffc8c-118">Další informace o chráněném zobrazení a o tom, jak změnit nastavení, najdete v tomto článku: [Co je chráněné zobrazení?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="ffc8c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="ffc8c-119">**Je OneDrive plný?**</span><span class="sxs-lookup"><span data-stu-id="ffc8c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="ffc8c-120">Pokud je soubor uložený na OneDrivu a máte zaplněný úložný prostor OneDrivu, nebude možné dokument uložit, dokud se nedosáhnou volného místa.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="ffc8c-121">Volné místo na OneDrivu můžete zkontrolovat tak, že v centru oznámení kliknete na ikonu OneDrive a vyberete Spravovat úložiště, nebo můžete přejít na , přihlásit se a poznamenat si množství využitých místa v levém dolním rohu [https://onedrive.live.com](https://onedrive.live.com) obrazovky.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="ffc8c-122">**Je Office aktivovaný?**</span><span class="sxs-lookup"><span data-stu-id="ffc8c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="ffc8c-123">Pokud Office není aktivovaný nebo vypršela platnost vašeho předplatného, můžete být v režimu omezené funkčnosti jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="ffc8c-124">Informace o aktivaci Office najdete v tématu: Chyby [nelicencovaných](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)produktů a aktivace v Office .</span><span class="sxs-lookup"><span data-stu-id="ffc8c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="ffc8c-125">**Pokud všechno ostatní selže...**</span><span class="sxs-lookup"><span data-stu-id="ffc8c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="ffc8c-126">Zkuste restartovat počítač.</span><span class="sxs-lookup"><span data-stu-id="ffc8c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="ffc8c-127">Instalace aktualizací Office</span><span class="sxs-lookup"><span data-stu-id="ffc8c-127">Install Office updates</span></span>
    
- <span data-ttu-id="ffc8c-128">Provedení online opravy Office</span><span class="sxs-lookup"><span data-stu-id="ffc8c-128">Perform an Online repair of Office</span></span>
    

