---
title: Řešení potíží se stávajícím monitorem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2ecfb4e90f2d58654ec43a35e901ea4421e0e94fa95995ef890abc8af2d99ec7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981070"
---
# <a name="troubleshoot-an-existing-monitor"></a>Poradce při potížích s existujícím monitorem

Vyzkoušejte tato řešení pro řešení potíží s monitorem. 

**Aktualizace zobrazení monitoru:**

Stiskněte současně následující klávesy: Windows + Ctrl + Shift + B. Tím se obnoví komunikace s ovladačem grafické karty. Vaše monitory budou na okamžik blikat a po několika sekundách se vrátí.

**Poradce při potížích s hardwarem monitoru:**

1. Odpojte kabel připojující počítač k monitoru a znovu ho připojte.
2. Odpojte všechna zařízení, která nejsou nezbytná, od počítače (například adaptéry nebo doky).

**Pokud jste nedávno nainstalovali aktualizaci na počítači, můžete ovladač zobrazení vrátit zpět:**

1. Vyberte **Start,** zadejte **Správce zařízení** a ve **výsledcích** vyberte Správce zařízení.
2. Rozbalte **část Grafické adaptéry,** klikněte pravým tlačítkem myši na grafický adaptér a vyberte **Vlastnosti**.
3. Přejděte na kartu **Ovladač** a vyberte **Vrátit ovladač zpět.** <br>
Poznámka: Pokud tato možnost není dostupná nebo  je šedě šedě, vyberte v následujících možnostech možnost Ne a přejděte k dalšímu kroku.
4. Možná budete muset restartovat počítač, než se tyto změny projeví.

**Odinstalace a přeinstalace ovladače zobrazení:**

1. Vyberte **Start,** zadejte **Správce zařízení** a ve **výsledcích** vyberte Správce zařízení.
2. Rozbalte **část Grafické adaptéry,** klikněte pravým tlačítkem myši na grafický adaptér a vyberte **Odinstalovat zařízení.** 
3. Zaškrtněte políčko Vedle možnosti **Odstranit software ovladače pro toto zařízení a** vyberte **Odinstalovat.**<br>
Poznámka: V této fázi se může zobrazit dotaz, jestli chcete restartovat počítač. Před restartováním si nezapomeňte zapsat zbývající pokyny.
4. Znovu otevřete Správce zařízení.
5. Rozbalte **část Grafické adaptéry,** klikněte pravým tlačítkem myši na grafický adaptér a vyberte **Aktualizovat ovladač.**
6. Vyberte **Automaticky hledat aktualizační software ovladače** a postupujte podle pokynů k instalaci.