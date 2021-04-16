---
title: Otázky k použití nástroje pro nasazení Office (ODT)
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
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790325"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky k použití nástroje pro nasazení Office (ODT)

Stáhněte si nástroj pro nasazení Office z [webu Stažení softwaru společnosti Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Po stažení souboru spusťte samo extrahovací spustitelný soubor, který obsahuje spustitelný soubor Nástroje pro nasazení Office (setup.exe) a ukázkový konfigurační soubor (configuration.xml).
  
 **Vyloučení nebo odebrání aplikací Microsoft 365 pro podnikové produkty z klientských počítačů:**
  
Při instalaci aplikací Microsoft 365 pro podniky můžete vyloučit konkrétní produkty. Postupujte podle pokynů pro instalaci Office pomocí funkce ODT, ale do konfiguračního souboru zahrnte element ExcludeApp. Tento konfigurační soubor například nainstaluje všechny aplikace Microsoft 365 pro podnikové produkty kromě Publisheru:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Přehled nástroje pro nasazení Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

