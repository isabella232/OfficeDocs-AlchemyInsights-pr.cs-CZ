---
title: Otázky týkající se používání nástroje pro nasazení Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086149"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="bf162-102">Otázky týkající se používání nástroje pro nasazení Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="bf162-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="bf162-103">Stáhněte si nástroj pro nasazení Office z [webu Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="bf162-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="bf162-104">Po stažení souboru spusťte samorozbalovací spustitelný soubor, který obsahuje spustitelný Nástroj pro nasazení Office (setupodt.exe) a ukázkový konfigurační soubor (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="bf162-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="bf162-105">**Vyloučení nebo odebrání aplikací Microsoft 365 pro podnikové produkty z klientských počítačů:**</span><span class="sxs-lookup"><span data-stu-id="bf162-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="bf162-106">Při instalaci aplikací Microsoft 365 pro podnik můžete vyloučit určité produkty.</span><span class="sxs-lookup"><span data-stu-id="bf162-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="bf162-107">Postupujte podle pokynů k instalaci Office pomocí ODT, ale do konfiguračního souboru se zahrne i element ExcludeApp.</span><span class="sxs-lookup"><span data-stu-id="bf162-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="bf162-108">Tento konfigurační soubor například nainstaluje všechny aplikace Microsoft 365 pro podnikové produkty s výjimkou aplikace Publisher:</span><span class="sxs-lookup"><span data-stu-id="bf162-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="bf162-109">Přehled nástroje pro nasazení Office</span><span class="sxs-lookup"><span data-stu-id="bf162-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

