---
title: Řízení automatických aktualizací pro aplikace Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747769"
---
# <a name="control-automatic-updates-for-office-apps"></a>Řízení automatických aktualizací pro aplikace Office

Ve výchozím nastavení se aktualizace aplikací Office automaticky stáhnou a použijí se na pozadí bez zásahu uživatele. Správci ale můžou řídit, jak se aktualizace používají pomocí nastavení Office Update. Nastavení aktualizací: umožňuje správcům povolit nebo zakázat automatické aktualizace, zobrazit nebo skrýt v Office tlačítko **aktualizovat** , nastavit termíny aktualizace a další. Podrobné informace najdete v těchto tématech:

- [Konfigurace nastavení aktualizací pro Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatická aktualizace Office není povolená.](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Určení způsobu aktualizace Office po instalaci](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Pokud chcete zkontrolovat nastavení existujících aktualizací použitých pro klientský počítač, postupujte takto:

1. Otevřete Editor registru **– Spusťte nástroj**  >  **Run**  >  **Regedit**.
2. Přejděte do následujícího umístění a zkontrolujte nastavení aktualizace Office:  
    a. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Poznámka:**  Pokud je nastaven klíč OfficeMgmtCOM, může se zobrazit zpráva "aktualizace jsou spravovány správcem systému **" v**  >  **Account**  >  **aktualizacích Office Account Updates**. Další informace najdete v článku [Správa aktualizací aplikací microsoft 365 pomocí nástroje Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  