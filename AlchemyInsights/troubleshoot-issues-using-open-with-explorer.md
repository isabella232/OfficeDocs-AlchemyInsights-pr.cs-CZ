---
title: Řešení problémů s používáním funkce Otevřít v Průzkumníkovi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323559"
---
# <a name="fix-problems-with-open-with-explorer"></a>Řešení problémů s aplikací Otevřít v Průzkumníkovi

Řešení běžných problémů s otevřením knihovny dokumentů v SharePoint nebo OneDrive pomocí **příkazu Otevřít v Průzkumníkovi:** 
  
- Použijte Internet Explorer 10 nebo Internet Explorer 11. **Otevřít v Průzkumníkovi** není kompatibilní s Microsoft Edge, Google Chrome, Firefoxem a dalšími. **Možnost Otevřít v Průzkumníkovi** je zakázaná ve všech prohlížečích kromě Internet Exploreru. 
    
- **Open with Explorer** is not available in the modern experience for SharePoint libraries. Místo **toho použijte Zobrazení v Průzkumníkovi** souborů. Vyberte **Zobrazit možnosti** Zobrazení v \> **Průzkumníkovi souborů**. Zobrazení v Průzkumníkovi souborů není kompatibilní s Microsoft Edge, Google Chrome, Firefoxem a dalšími uživateli. **Zobrazení v Průzkumníkovi souborů** je dostupné jenom v Internet Exploreru. 
    
- Zkontrolujte, jestli je služba Webový klient spuštěná. Do vyhledávacího Windows zadejte spustit, vyberte desktopovou aplikaci Spustit, zadejte services.msc a stiskněte Enter. Posuňte se dolů ke službě Webový klient a ujistěte se, že ve **sloupci Stav** se zobrazuje "Spuštěno". Pokud ne, poklikejte na službu, klikněte na **Start** a potom klikněte na **OK.** (Možná budete muset službu nejdřív povolit  tak, že v poli Typ spouštění vyberete Ručně nebo **Automaticky.)**  
    
**Poznámka:** Otevření knihovny v Průzkumníkovi souborů je šikovné, pokud potřebujete zkopírovat nebo přesunout více souborů a složek jednou, ale pokud chcete v knihovně pravidelně pracovat, doporučujeme ji synchronizovat. Pokud chcete vyřešit problémy s otevřením v Průzkumníkovi souborů, podívejte [se na článek Otevření v Průzkumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Informace o nastavení synchronizace najdete v tématu Synchronizace [SharePoint souborů s novým synchronizační aplikace OneDrivu klienta.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Další informace najdete v článku Použití příkazu Otevřít v Průzkumníkovi k řešení problémů [SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

