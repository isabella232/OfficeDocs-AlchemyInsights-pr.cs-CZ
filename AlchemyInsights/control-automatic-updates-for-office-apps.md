---
title: Řízení automatických aktualizací Office aplikací
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
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929874"
---
# <a name="control-automatic-updates-for-office-apps"></a>Řízení automatických aktualizací Office aplikací

Ve výchozím nastavení se aktualizace Office aplikace stahují automaticky a použijí se na pozadí bez zásahu uživatele. Správci ale můžou řídit způsob použití aktualizací pomocí Office Nastavení aktualizace. Nastavení aktualizací umožňují správcům povolit nebo zakázat  automatické aktualizace, zobrazit nebo skrýt tlačítko Aktualizovat v Office, nastavit konečné termíny aktualizace a další. Podrobné informace najdete v následujících článcích:

- [Konfigurace nastavení aktualizace pro Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatická aktualizace pro Office není povolená.](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definování Office aktualizace po instalaci](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Pokud chcete zkontrolovat stávající nastavení aktualizací použité na klientském počítači, postupujte takto:To review the existing updates settings applied to a client machine, follow these steps:

1. Otevřete Editor registru tak, že půjdete na **Spustit**  >    >  **spustit regedit**.
2. Přejděte do následujícího umístění a zkontrolujte nastavení Office Aktualizace:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Poznámka:**  Pokud je klíč OfficeMgmtCOM nastavený, může se v Office Account Office Updates zobrazit zpráva "Aktualizace jsou spravovány vaším  >    >  **správce systému".** Další informace najdete v tématu [Správa aktualizací Microsoft 365 Apps s Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  