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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774884"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Otázky týkající se používání nástroje pro nasazení Office (ODT)

Stáhněte si nástroj pro nasazení Office z [webu Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po stažení souboru spusťte samorozbalovací spustitelný soubor, který obsahuje spustitelný Nástroj pro nasazení Office (setup.exe) a ukázkový konfigurační soubor (configuration.xml).
  
 **Vyloučení nebo odebrání aplikací Microsoft 365 pro podnikové produkty z klientských počítačů:**
  
Při instalaci aplikací Microsoft 365 pro podnik můžete vyloučit určité produkty. Postupujte podle pokynů k instalaci Office pomocí ODT, ale do konfiguračního souboru se zahrne i element ExcludeApp. Tento konfigurační soubor například nainstaluje všechny aplikace Microsoft 365 pro podnikové produkty s výjimkou aplikace Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Přehled nástroje pro nasazení Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

