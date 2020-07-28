---
title: Řízení automatických aktualizací pro aplikace Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438839"
---
# <a name="control-automatic-updates-for-office-apps"></a>Řízení automatických aktualizací pro aplikace Office

Ve výchozím nastavení se aktualizace aplikací Office stahují automaticky a aplikují se na pozadí bez zásahu uživatele. Správci však mohou řídit způsob použití aktualizací pomocí nastavení služby Office Update. Nastavení aktualizací umožňuje správcům povolit nebo zakázat automatické aktualizace, zobrazit nebo skrýt tlačítko **Aktualizovat** v Office, nastavit termíny aktualizace a další. Podrobné informace naleznete v tématu:

- [Konfigurace nastavení aktualizací pro Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatické aktualizace pro Office nejsou povoleny.](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definování způsobu aktualizace Office po instalaci](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Chcete-li zkontrolovat existující nastavení aktualizací použitá pro klientský počítač, postupujte takto:

1. Otevřete Editor registru tak, že přejdete na **spustit**  >  **Run**  >  **spustit regedit**.
2. Přepněte do následujícího umístění a zkontrolujte nastavení Office Update:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Konfigurace

**Poznámka:**  Pokud je klíč OfficeMgmtCOM nastavený, může se v **Office**  >  **aktualizacích sady**Office Office zobrazit zpráva "Aktualizace jsou spravovány správcem systému"  >  **Office Updates**. Další informace najdete v [tématu Správa aktualizací aplikací Microsoft 365 pomocí Nástroje pro konfiguračního bodu Microsoft.](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)  