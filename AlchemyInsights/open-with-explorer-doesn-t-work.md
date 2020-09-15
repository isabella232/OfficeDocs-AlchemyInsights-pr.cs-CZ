---
title: Otevření v Průzkumníkovi nefunguje
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694449"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="9712b-102">Otevření v Průzkumníkovi nefunguje</span><span class="sxs-lookup"><span data-stu-id="9712b-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="9712b-103">Pokud **otevření v Průzkumníkovi** nebo **zobrazení v Průzkumníkovi souborů** nefunguje, zkontrolujte, jestli je služba Webový klient nastavená tak, aby **běžela** podle následujícího postupu.</span><span class="sxs-lookup"><span data-stu-id="9712b-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="9712b-104">Může to například trvat dlouhou dobu, když budete chtít otevřít SharePoint nebo knihovnu OneDrive, když služba není spuštěná.</span><span class="sxs-lookup"><span data-stu-id="9712b-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="9712b-105">Do pole Windows Search zadejte příkaz Spustit, vyberte spustit desktopovou aplikaci, zadejte Services. msc a pak vyberte **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="9712b-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="9712b-106">Posuňte se dolů ke službě Webový klient a zkontrolujte sloupec **stav** .</span><span class="sxs-lookup"><span data-stu-id="9712b-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="9712b-107">Pokud služba Webový klient **neběží**, poklikejte na ni, klikněte na **Start**a potom klikněte na **OK**.</span><span class="sxs-lookup"><span data-stu-id="9712b-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9712b-108">V případě potřeby tuto službu povolte výběrem možnosti **ručně** nebo **automaticky** v poli **Typ spouštění** .</span><span class="sxs-lookup"><span data-stu-id="9712b-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9712b-109">Informace o řešení problémů s otevřením v Průzkumníkovi souborů najdete v článku [otevření v Průzkumníkovi](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="9712b-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9712b-110">Prozkoumejte synchronizaci jako lepší alternativu: [synchronizace sharepointových souborů pomocí nového synchronizačního klienta OneDrivu](https://go.microsoft.com/fwlink/?linkid=871666)</span><span class="sxs-lookup"><span data-stu-id="9712b-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

