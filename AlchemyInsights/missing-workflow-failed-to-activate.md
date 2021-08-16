---
title: Aktivace chybějícího pracovního postupu se nezdařila.
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065421"
---
# <a name="missing-workflow-failed-to-activate"></a>Aktivace chybějícího pracovního postupu se nezdařila.

V kolekci webů Microsoft SharePoint nelze přidat globálně znovu použitelný pracovní postup (například "Schválení – SharePoint 2010") do seznamu nebo knihovny.
  
Tento problém vyřešíte takto: 
  
1. Otevřete kořenový web kolekce webů v SharePoint Designer 2013.
  
2. V **části Objekty webu** vyberte Pracovní **postupy**. 
  
3. V části **Nový** na pásu karet **Pracovní** postupy vyberte **Znovu použitelný pracovní postup**. 
  
4. Ve formuláři **Vytvořit znovu použitelný pracovní** postup zadejte název ** *Oprava2010* **. V **seznamu Typ platformy** klikněte na SharePoint pracovního postupu **2010** a potom klikněte na **OK.** 
  
1. V části **Uložit** na pásu karet **Pracovního** postupu vyberte **Publikovat**. 
  
2. V části **Manage** (Spravovat) na **pásu** karet Pracovního postupu vyberte **Publish Globally (Publikovat globálně).** V potvrzovacím dialogovém okně, které se zobrazí, vyberte **OK.** 
  
3. Ve webovém prohlížeči vyhledejte kořenový web kolekce webů a potom přejděte na Web **Nastavení** \> **funkce kolekce webů**. Potom přepněte funkci **Pracovní** postupy: 
  
· Pokud je tato funkce *aktivovaná,* klikněte na **Deaktivovat** a potom klikněte na **Aktivovat.** 
  
· Pokud je funkce *deaktivovaná,* klikněte na **Aktivovat.** 
  
Další informace najdete v následujícím [článku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

