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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794904"
---
# <a name="using-the-office-deployment-tool-odt"></a>Použití nástroje pro nasazení Office (ODT)

K nasazení Office 365 verze Office se používá nástroj pro nasazení Office (ODT). Nástroj pro nasazení Office (setup.exe) se spouští z příkazového řádku a pomocí konfiguračního souboru XML zjistíte, jaké nastavení se použije při nasazení Office.
  
1. Stáhněte si nejnovější verzi nástroje pro nasazení Office z [webu Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Pomocí [Nástroje pro přizpůsobení Office (OCT)](https://config.office.com) vyberte Předvolby nasazení a vytvořte konfigurační soubor XML. Exportujte konfigurační soubor a umístěte ho místně do stejné složky, kde se setup.exe nachází.

    **Poznámka:** Problémy s instalací Office se obvykle vyskytují v důsledku chybně nakonfigurovaných nebo malformatted konfiguračních souborů. Abyste předešli těmto problémům, doporučujeme vytvořit konfigurační soubor pomocí nástroje pro přizpůsobení Office. Můžete taky importovat stávající konfigurační soubory do nástroje pro přizpůsobení Office.

3. Na příkazovém řádku se zvýšenými oprávněními přejděte do umístění, kde se setup.exe nachází, a spusťte nástroj pro nasazení Office v režimu stahování a zadejte konfigurační soubor, který jste právě uložili. V tomto příkladu je konfigurační soubor pojmenovaný Configuration.xml:

```setup.exe /download Configuration.xml```

4. Spusťte nástroj pro nasazení Office v režimu konfigurace a určete konfigurační soubor.

```setup.exe /configure Configuration.xml```

**Poznámka:** Tento krok musíte spustit z klientského počítače, na který chcete nainstalovat Office, a musíte mít na tomto počítači oprávnění místního správce.

Další informace o používání nástroje pro nasazení Office pro aplikace Microsoft 365 pro podnikové scénáře nasazení pro podniky najdete v tématu [Přehled nástroje pro nasazení Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Další podrobnosti o používání nástroje pro přizpůsobení Office najdete v tématu [Přehled nástroje pro přizpůsobení Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
