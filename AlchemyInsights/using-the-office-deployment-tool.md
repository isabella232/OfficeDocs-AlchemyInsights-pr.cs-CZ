---
title: Použití nástroje pro nasazení Office
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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085825"
---
# <a name="using-the-office-deployment-tool-odt"></a>Použití nástroje pro nasazení Office (ODT)

K nasazení Office 365 verze Office se používá nástroj pro nasazení Office (ODT). Nástroj pro nasazení Office (setupodt.exe) se spouští z příkazového řádku a pomocí konfiguračního souboru XML zjistíte, jaké nastavení se použije při nasazení Office.
  
1. Stáhněte si nejnovější verzi nástroje pro nasazení Office z [webu Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Pomocí [Nástroje pro přizpůsobení Office (OCT)](https://config.office.com) vyberte Předvolby nasazení a vytvořte konfigurační soubor XML. Exportujte konfigurační soubor a umístěte ho místně do stejné složky, kde se setupodt.exe nachází.

    **Poznámka:** Problémy s instalací Office se obvykle vyskytují v důsledku chybně nakonfigurovaných nebo malformatted konfiguračních souborů. Abyste předešli těmto problémům, doporučujeme vytvořit konfigurační soubor pomocí nástroje pro přizpůsobení Office. Můžete taky importovat stávající konfigurační soubory do nástroje pro přizpůsobení Office.

3. Na příkazovém řádku se zvýšenými oprávněními přejděte do umístění, kde se setupodt.exe nachází, a spusťte nástroj pro nasazení Office v režimu stahování a zadejte konfigurační soubor, který jste právě uložili. V tomto příkladu je konfigurační soubor pojmenovaný Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Spusťte nástroj pro nasazení Office v režimu konfigurace a určete konfigurační soubor.

```setupodt.exe /configure Configuration.xml```

**Poznámka:** Tento krok musíte spustit z klientského počítače, na který chcete nainstalovat Office, a musíte mít na tomto počítači oprávnění místního správce.

Další informace o používání nástroje pro nasazení Office pro aplikace Microsoft 365 pro podnikové scénáře nasazení pro podniky najdete v tématu [Přehled nástroje pro nasazení Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Další podrobnosti o používání nástroje pro přizpůsobení Office najdete v tématu [Přehled nástroje pro přizpůsobení Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
