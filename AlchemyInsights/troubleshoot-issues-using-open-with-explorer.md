---
title: Poradce při potížích s používáním funkce Otevřít v Průzkumníkovi
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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048149"
---
# <a name="fix-problems-with-open-with-explorer"></a>Řešení problémů s aplikací Otevřít v Průzkumníkovi

Řešení běžných problémů s otevřením knihovny dokumentů v SharePoint nebo OneDrive pomocí **příkazu Otevřít v Průzkumníkovi:** 
  
- Použijte Internet Explorer 10 nebo Internet Explorer 11. **Otevřít v Průzkumníkovi** není kompatibilní s Microsoft Edge, Google Chrome, Firefoxem a dalšími. **Možnost Otevřít v Průzkumníkovi** je zakázaná ve všech prohlížečích kromě Internet Exploreru. 
    
- **Open with Explorer** is not available in the modern experience for SharePoint libraries. Místo **toho použijte Zobrazení v Průzkumníkovi** souborů. Vyberte **Zobrazit možnosti** Zobrazení v \> **Průzkumníkovi souborů**. Zobrazení v Průzkumníkovi souborů není kompatibilní s Microsoft Edge, Google Chrome, Firefoxem a dalšími uživateli. **Zobrazení v Průzkumníkovi souborů** je dostupné jenom v Internet Exploreru. 
    
- Zkontrolujte, jestli je služba Webový klient spuštěná. Do vyhledávacího Windows zadejte spustit, vyberte desktopovou aplikaci Spustit, zadejte services.msc a stiskněte Enter. Posuňte se dolů ke službě Webový klient a ujistěte se, že ve **sloupci Stav** se zobrazuje "Spuštěno". Pokud ne, poklikejte na službu, klikněte na **Start** a potom klikněte na **OK.** (Možná budete muset službu nejdřív povolit  tak, že v poli Typ spouštění vyberete Ručně nebo **Automaticky.)**  
    
> [!NOTE]
> Otevření knihovny v Průzkumníkovi souborů je vhod, pokud potřebujete zkopírovat nebo přesunout více souborů a složek jednou, ale pokud chcete v knihovně pravidelně pracovat, doporučujeme ji synchronizovat. Pokud chcete vyřešit problémy s otevřením v Průzkumníkovi souborů, podívejte [se na článek Otevření v Průzkumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Informace o nastavení synchronizace najdete v tématu Synchronizace [SharePoint souborů s novým synchronizační aplikace OneDrivu klienta](https://go.microsoft.com/fwlink/?linkid=871666).
  
Další informace najdete v článku Použití příkazu Otevřít v Průzkumníkovi k řešení problémů [SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

