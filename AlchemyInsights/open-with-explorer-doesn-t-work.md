---
title: Otevřít v Průzkumníkovi nefunguje
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321854"
---
# <a name="open-with-explorer-isnt-working"></a>Nefunguje otevřít v Průzkumníkovi

Pokud **funkce Otevřít v Průzkumníkovi** nebo Zobrazení v Průzkumníkovi souborů  nefunguje, zkontrolujte, jestli je služba Webový klient nastavená na Spuštěno podle následujících kroků.  Například může trvat dlouho, než otevřete knihovnu SharePoint nebo OneDrive, když služba není spuštěná. 
  
1. Do vyhledávacího Windows zadejte spustit, vyberte desktopová aplikace Spustit, zadejte services.msc a pak vyberte **Enter**.
    
2. Posuňte se dolů ke službě Webový klient a zkontrolujte **sloupec** Stav. Pokud stav služby Webový klient není **spuštěný,** poklikejte na službu, klikněte na **Start** a potom klikněte na **OK.** V případě potřeby službu povolte  tak, že v poli Typ spouštění vyberete ručně nebo **automaticky.**  
    
**Poznámka:** Pokud chcete vyřešit problémy s otevřením v Průzkumníkovi souborů, podívejte [se na článek Otevření v Průzkumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Prozkoumejte synchronizaci jako lepší alternativu: Synchronizace SharePoint souborů s novým synchronizační aplikace OneDrivu [klientem](https://go.microsoft.com/fwlink/?linkid=871666). 
  

