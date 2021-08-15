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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011329"
---
# <a name="open-with-explorer-isnt-working"></a>Nefunguje otevřít v Průzkumníkovi

Pokud **funkce Otevřít v Průzkumníkovi** nebo Zobrazení v Průzkumníkovi souborů  nefunguje, zkontrolujte, jestli je služba Webový klient nastavená na Spuštěno podle následujících kroků.  Například může trvat dlouho, než otevřete knihovnu SharePoint nebo OneDrive, když služba není spuštěná. 
  
1. Do vyhledávacího Windows zadejte spustit, vyberte desktopová aplikace Spustit, zadejte services.msc a pak vyberte **Enter**.
    
2. Posuňte se dolů ke službě Webový klient a zkontrolujte **sloupec** Stav. Pokud stav služby Webový klient není **spuštěný,** poklikejte na službu, klikněte na **Start** a potom klikněte na **OK.** V případě potřeby službu povolte  tak, že v poli Typ spouštění vyberete ručně nebo **automaticky.**  
    
> [!NOTE]
> Pokud chcete vyřešit problémy s otevřením v Průzkumníkovi souborů, podívejte [se na článek Otevření v Průzkumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Prozkoumejte synchronizaci jako lepší alternativu: Synchronizace SharePoint souborů s novým synchronizační aplikace OneDrivu [klientem](https://go.microsoft.com/fwlink/?linkid=871666). 
  

