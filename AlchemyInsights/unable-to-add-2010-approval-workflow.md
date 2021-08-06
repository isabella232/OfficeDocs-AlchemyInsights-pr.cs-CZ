---
title: Pracovní postup schválení 2010 se nedaří přidat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020329"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Pracovní postup schválení 2010 se nedaří přidat

V kolekci webů Microsoft SharePoint nelze přidat globálně znovu použitelný pracovní postup (například "Schválení – SharePoint 2010") do seznamu nebo knihovny.
  
Tento problém vyřešíte takto: 
  
1. Otevřete kořenový web kolekce webů v SharePoint Designer 2013.
  
2. V **části Objekty webu** vyberte Pracovní **postupy**. 
  
3. V části **Nový** na pásu karet **Pracovní** postupy vyberte **Znovu použitelný pracovní postup**. 
  
4. Ve formuláři **Vytvořit znovu použitelný pracovní** postup zadejte název ** *Oprava2010* **. V **seznamu Typ platformy** klikněte na SharePoint pracovního postupu **2010** a potom klikněte na **OK.** 
  
1. V části **Uložit** na pásu karet **Pracovního** postupu vyberte **Publikovat**. 
  
2. V části **Manage** (Spravovat) na **pásu** karet Pracovního postupu vyberte **Publish Globally (Publikovat globálně).** V potvrzovacím dialogovém okně, které se zobrazí, vyberte **OK.** 
  
3. Ve webovém prohlížeči vyhledejte kořenový web kolekce webů a potom přejděte na Web **Nastavení** \> **funkce kolekce webů**. Přepnutí funkce **Pracovní** postupy: 
  
· Pokud je tato funkce *aktivovaná,* klikněte na **Deaktivovat** a potom klikněte na **Aktivovat.** 
  
· Pokud je funkce *deaktivovaná,* klikněte na **Aktivovat.** 
  
Další informace najdete v následujícím [článku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

