---
title: Poradce při potížích s používáním aplikace Open Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659051"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="61ad6-102">Řešení problémů s programem otevřít v Průzkumníkovi</span><span class="sxs-lookup"><span data-stu-id="61ad6-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="61ad6-103">Řešení běžných problémů při otevírání knihovny dokumentů na SharePointu nebo OneDrivu pomocí příkazu **otevřít v Průzkumníkovi** :</span><span class="sxs-lookup"><span data-stu-id="61ad6-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="61ad6-104">Použijte Internet Explorer 10 nebo Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="61ad6-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="61ad6-105">Příkaz **otevřít v Průzkumníkovi** není kompatibilní s Microsoft Edgem, Google Chrome, Firefox a dalšími lidmi.</span><span class="sxs-lookup"><span data-stu-id="61ad6-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="61ad6-106">**Otevření** v aplikaci Explorer je zakázáno ve všech prohlížečích s výjimkou Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="61ad6-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="61ad6-107">Možnost **otevřít v Průzkumníkovi** není dostupná v moderních prostředích pro sharepointové knihovny.</span><span class="sxs-lookup"><span data-stu-id="61ad6-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="61ad6-108">Místo toho použijte **zobrazení v Průzkumníkovi souborů** .</span><span class="sxs-lookup"><span data-stu-id="61ad6-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="61ad6-109">**View options** \> **V Průzkumníkovi souborů vyberte zobrazení**možnosti zobrazení.</span><span class="sxs-lookup"><span data-stu-id="61ad6-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="61ad6-110">Zobrazení v Průzkumníkovi souborů není kompatibilní s Microsoft Edgem, Google Chrome, Firefox a dalšími lidmi.</span><span class="sxs-lookup"><span data-stu-id="61ad6-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="61ad6-111">**Zobrazení v Průzkumníkovi souborů** v Internet Exploreru</span><span class="sxs-lookup"><span data-stu-id="61ad6-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="61ad6-112">Ujistěte se, že služba Webový klient běží.</span><span class="sxs-lookup"><span data-stu-id="61ad6-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="61ad6-113">Do pole Windows Search zadejte příkaz Spustit, vyberte spustit desktopovou aplikaci, zadejte Services. msc a stiskněte ENTER.</span><span class="sxs-lookup"><span data-stu-id="61ad6-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="61ad6-114">Posuňte se dolů na službu Webový klient a ujistěte se, že sloupec **stav** zobrazuje "spouští se".</span><span class="sxs-lookup"><span data-stu-id="61ad6-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="61ad6-115">Pokud není, poklikejte na ni, klikněte na **Start**a potom klikněte na **OK**.</span><span class="sxs-lookup"><span data-stu-id="61ad6-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="61ad6-116">(Tuto službu bude pravděpodobně nutné nejprve povolit výběrem možnosti **ručně** nebo **automaticky** v poli **Typ spouštění** .)</span><span class="sxs-lookup"><span data-stu-id="61ad6-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="61ad6-117">Otevření knihovny v Průzkumníkovi souborů je užitečné, pokud potřebujete zkopírovat nebo přesunout více souborů a složek jednou, ale pokud chcete v knihovně pravidelně pracovat, doporučujeme to synchronizovat.</span><span class="sxs-lookup"><span data-stu-id="61ad6-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="61ad6-118">Informace o řešení problémů s otevřením v Průzkumníkovi souborů najdete v článku [otevření v Průzkumníkovi](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="61ad6-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="61ad6-119">Informace o nastavení synchronizace najdete v článku [synchronizace sharepointových souborů pomocí nového synchronizačního klienta OneDrivu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="61ad6-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="61ad6-120">Další informace najdete v článku [použití příkazu otevřít v Průzkumníkovi k řešení problémů v SharePointu Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="61ad6-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

