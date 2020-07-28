---
title: Změna kanálů aktualizací pro aplikace Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438855"
---
# <a name="change-update-channels-for-office-apps"></a>Změna kanálů aktualizací pro aplikace Office

U nových instalací Office vyberte požadovaný kanál aktualizace pomocí nastavení stahování softwaru Office a pak nainstalujte (nebo znovu nainstalujte) aplikace Office. Další informace najdete [v tématu Správa nastavení stahování softwaru v Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Poznámka:** Kanál aktualizace vybraný pomocí nastavení stahování softwaru Office se vztahuje na všechny uživatele, kteří provádějí nové instalace pomocí portálu O365. Další informace najdete v [tématu Stažení a instalace nebo přeinstalace Microsoftu 365 nebo Office 2019 na PC nebo Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

U stávajících instalací Office přepněte na jiný kanál aktualizace pomocí nástroje OFFICE Deployment Tool (ODT):  

1. Stáhněte si nejnovější verzi Nástroje pro nasazení sady Office (setup.exe) ze [služby Stažení softwaru](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Určete název kanálu, na který chcete přepnout. Další informace naleznete [v tématu Možnosti konfigurace nástroje pro nasazení sady Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Vytvořte konfigurační soubor XML určující příslušný název kanálu, například update.xml.  
    a. <Configuration>  
    b. <aktualizace **Channel="Měsíčně"** />  
    c. </Configuration>
4. Z příkazového řádku se zvýšenými oprávněními přepněte do umístění složky, kde setup.exe, a spusťte následující příkaz:  
    a. setup.exe /configure update.xml
5. Spusťte aplikaci Office (například Excel) a pak vyberte **Účet souborů**  >  **Account**. V části Informace o produktu vyberte **možnosti**  >  **aktualizace Aktualizovat nyní**.

Další informace naleznete v [tématu Jak přepnout kanály aktualizací pro existující aplikace Office .](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) 

Chcete-li přepnout aktualizační kanály pro vybranou skupinu uživatelů nebo pomocí nástroje Configuration Manager (SCCM), nakonfigurujte nastavení Aktualizovat kanál pomocí objektu zásad skupiny. Další informace najdete v [tématu Přehled kanálů aktualizací aplikací Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Podrobnosti najdete v [tématu Správa kanálů Office 365 ProPlus pro IT profesionály](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) a [správa aktualizací aplikací Microsoft 365 pomocí Nástroje pro konfiguraci koncových bodů Microsoft](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).