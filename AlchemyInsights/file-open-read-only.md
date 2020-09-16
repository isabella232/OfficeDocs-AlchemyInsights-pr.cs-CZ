---
title: Otevření souboru jen pro čtení
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745569"
---
# <a name="file-open-read-only"></a><span data-ttu-id="3577e-102">Otevření souboru jen pro čtení</span><span class="sxs-lookup"><span data-stu-id="3577e-102">File open read-only</span></span>

<span data-ttu-id="3577e-103">Můžete zjistit, že když soubory otvíráte, otevřou se jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="3577e-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="3577e-104">V některých případech jde o přidanou bezpečnost, třeba když otvíráte soubory z Internetu, a jindy to může být způsobeno nastavením, které se dá změnit.</span><span class="sxs-lookup"><span data-stu-id="3577e-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="3577e-105">Tady je několik situací, kdy se soubor otevře jen pro čtení, a některé kroky, které můžete změnit.</span><span class="sxs-lookup"><span data-stu-id="3577e-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="3577e-106">**Můj antivirový program způsobuje, že je otevře jen pro čtení**</span><span class="sxs-lookup"><span data-stu-id="3577e-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="3577e-107">Některé antivirové programy můžou chránit před potenciálně nebezpečnými soubory jejich otevřením jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="3577e-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="3577e-108">Pokud chcete zjistit, jak se tato nastavení upraví, obraťte se na svého poskytovatele antivirového softwaru.</span><span class="sxs-lookup"><span data-stu-id="3577e-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="3577e-109">BitDefender například obsahuje obsah týkající se přidávání vyloučení aplikací tady: [jak přidat vyloučení aplikací nebo procesů v ovládacím centru BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="3577e-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="3577e-110">**Jsou vlastnosti souboru nastavené na jen pro čtení?**</span><span class="sxs-lookup"><span data-stu-id="3577e-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="3577e-111">Vlastnosti souboru můžete zkontrolovat tak, že kliknete pravým tlačítkem na soubor a vyberete vlastnosti.</span><span class="sxs-lookup"><span data-stu-id="3577e-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="3577e-112">Pokud je zaškrtnuté políčko atribut jen pro čtení, zrušte jeho zaškrtnutí a klikněte na OK.</span><span class="sxs-lookup"><span data-stu-id="3577e-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="3577e-113">**Obsah je v chráněném zobrazení**</span><span class="sxs-lookup"><span data-stu-id="3577e-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="3577e-114">Soubory z Internetu a z jiných potenciálně nebezpečných umístění můžou obsahovat viry, červy nebo jiné druhy malwaru, které můžou poškodit váš počítač.</span><span class="sxs-lookup"><span data-stu-id="3577e-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="3577e-115">Obvykle se to týká i příloh e-mailů nebo stažených souborů.</span><span class="sxs-lookup"><span data-stu-id="3577e-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="3577e-116">Z důvodu ochrany počítače se soubory z těchto potenciálně nebezpečných umístění otevřou v chráněném zobrazení.</span><span class="sxs-lookup"><span data-stu-id="3577e-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="3577e-117">V chráněném zobrazení si můžete přečíst soubor a zobrazit jeho obsah a současně snížit riziko.</span><span class="sxs-lookup"><span data-stu-id="3577e-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="3577e-118">Další informace o chráněném zobrazení a změnách nastavení najdete v tomto článku: [co je chráněné zobrazení?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="3577e-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="3577e-119">**Je OneDrive zaplněný?**</span><span class="sxs-lookup"><span data-stu-id="3577e-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="3577e-120">Pokud je soubor uložený na OneDrivu a prostor úložiště OneDrivu je zaplněný, nebudete moct dokument uložit, dokud nebudete pod vyhrazeným prostorem.</span><span class="sxs-lookup"><span data-stu-id="3577e-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="3577e-121">Pokud chcete zjistit, jestli máte volné místo na OneDrivu, klikněte na ikonu OneDrivu v centru oznámení a vyberte Spravovat úložiště, nebo můžete přejít na [https://onedrive.live.com](https://onedrive.live.com) , přihlásit se a zaznamenat množství využitého místa v levém dolním rohu obrazovky.</span><span class="sxs-lookup"><span data-stu-id="3577e-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="3577e-122">**Je Office aktivovaný?**</span><span class="sxs-lookup"><span data-stu-id="3577e-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="3577e-123">Pokud Office není aktivovaný, nebo pokud platnost vašeho předplatného vypršela, můžete být v režimu jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="3577e-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="3577e-124">Informace o tom, jak aktivovat Office, najdete v tématu: [chyby typu nelicencovaný produkt a chyby aktivace v Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="3577e-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="3577e-125">**Pokud všechny další selžou...**</span><span class="sxs-lookup"><span data-stu-id="3577e-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="3577e-126">Zkuste restartovat počítač</span><span class="sxs-lookup"><span data-stu-id="3577e-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="3577e-127">Instalace aktualizací Office</span><span class="sxs-lookup"><span data-stu-id="3577e-127">Install Office updates</span></span>
    
- <span data-ttu-id="3577e-128">Provedení online opravy Office</span><span class="sxs-lookup"><span data-stu-id="3577e-128">Perform an Online repair of Office</span></span>
    

