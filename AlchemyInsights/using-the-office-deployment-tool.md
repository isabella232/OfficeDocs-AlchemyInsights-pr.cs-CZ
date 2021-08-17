---
title: Použití nástroje Office nasazení
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083763"
---
# <a name="using-the-office-deployment-tool-odt"></a>Použití nástroje Office nasazení (ODT)

Nástroj pro nasazení Office (ODT) se používá k nasazení Office 365 verzí Office. Nástroj Office nasazení (setup.exe) se spustí z příkazového řádku a pomocí konfiguračního souboru XML určí, jaká nastavení se mají použít při nasazení Office.
  
1. Stáhněte si nejnovější verzi nástroje pro Office nasazení z [webu Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Pomocí nástroje [Office přizpůsobení (OCT)](https://config.office.com) vyberte předvolby nasazení a vytvořte konfigurační soubor XML. Exportujte konfigurační soubor a místně ho umístěte do stejné složky, ve které je setup.exe soubor.

    **Poznámka:** Office k problémům s instalací často dochází kvůli chybně nakonfigurovaným nebo chybně formátovaných konfiguračním souborům. Abyste se takovým problémům vyhnuli, doporučujeme k vytvoření konfiguračního souboru použít nástroj Office přizpůsobení. Existující konfigurační soubory můžete také importovat do nástroje Office přizpůsobení.

3. Z příkazového řádku se zvýšenými oprávněními přepněte do umístění, kde setup.exe, a spusťte nástroj pro nasazení Office v režimu stahování a zadejte právě uložený konfigurační soubor. V tomto příkladu se konfigurační soubor jmenuje Configuration.xml:

```setup.exe /download Configuration.xml```

4.Spusťte nástroj Office nasazení v režimu konfigurace a zadejte konfigurační soubor.

```setup.exe /configure Configuration.xml```

**Poznámka:** Tento krok musíte spustit z klientského počítače, na který chcete nainstalovat Office a musíte mít oprávnění místního správce v tomto počítači.

Další informace o použití nástroje Office nasazení pro Microsoft 365 Apps pro velké organizace nasazení najdete v tématu Přehled nástroje [Office nasazení.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Další informace o tom, jak používat nástroj Office přizpůsobení, najdete v tématu Přehled nástroje [Office přizpůsobení.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
