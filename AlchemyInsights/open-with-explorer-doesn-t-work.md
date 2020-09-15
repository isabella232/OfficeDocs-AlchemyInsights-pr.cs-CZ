---
title: Otevření v Průzkumníkovi nefunguje
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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694449"
---
# <a name="open-with-explorer-isnt-working"></a>Otevření v Průzkumníkovi nefunguje

Pokud **otevření v Průzkumníkovi** nebo **zobrazení v Průzkumníkovi souborů** nefunguje, zkontrolujte, jestli je služba Webový klient nastavená tak, aby **běžela** podle následujícího postupu. Může to například trvat dlouhou dobu, když budete chtít otevřít SharePoint nebo knihovnu OneDrive, když služba není spuštěná. 
  
1. Do pole Windows Search zadejte příkaz Spustit, vyberte spustit desktopovou aplikaci, zadejte Services. msc a pak vyberte **ENTER**.
    
2. Posuňte se dolů ke službě Webový klient a zkontrolujte sloupec **stav** . Pokud služba Webový klient **neběží**, poklikejte na ni, klikněte na **Start**a potom klikněte na **OK**. V případě potřeby tuto službu povolte výběrem možnosti **ručně** nebo **automaticky** v poli **Typ spouštění** . 
    
> [!NOTE]
> Informace o řešení problémů s otevřením v Průzkumníkovi souborů najdete v článku [otevření v Průzkumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Prozkoumejte synchronizaci jako lepší alternativu: [synchronizace sharepointových souborů pomocí nového synchronizačního klienta OneDrivu](https://go.microsoft.com/fwlink/?linkid=871666) 
  

