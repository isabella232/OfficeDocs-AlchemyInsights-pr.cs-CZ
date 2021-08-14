---
title: Otázky týkající se použití nástroje Office nasazení (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959676"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky týkající se použití nástroje Office nasazení (ODT)

Stáhněte si Office nástroj pro nasazení softwaru z [webu Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po stažení souboru spusťte samo extrahovací spustitelný soubor, který obsahuje spustitelný soubor nástroje Office Deployment Tool (setup.exe) a ukázkový konfigurační soubor (configuration.xml).
  
 **Vyloučení nebo odebrání Microsoft 365 Apps pro velké organizace z klientských počítačů:**
  
Při instalaci Microsoft 365 Apps pro velké organizace můžete vyloučit konkrétní produkty. Pokud to chcete udělat, postupujte podle pokynů pro instalaci Office pomocí funkce ODT, ale do konfiguračního souboru zahrnte element ExcludeApp. Tento konfigurační soubor například nainstaluje všechny produkty Microsoft 365 Apps pro velké organizace kromě Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Přehled nástroje Office nasazení](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

