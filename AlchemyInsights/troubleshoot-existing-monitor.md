---
title: Řešení potíží s existujícím monitorem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690704"
---
# <a name="troubleshoot-an-existing-monitor"></a>Řešení potíží s existujícím monitorem

Pokud chcete vyřešit problém s monitorem, vyzkoušejte tato řešení. 

**Aktualizace zobrazení monitoru:**

Současně stiskněte tyto klávesy: Klávesa Windows + CTRL + SHIFT + B. Touto akcí obnovíte komunikaci s grafickým ovladačem. Monitory se budou za chvíli blikat a po několika sekundách se zase odeberou.

**Řešení potíží s hardwarem monitoru:**

1. Odpojte kabel spojující počítač s monitorem a zapojte ho zpátky.
2. Odpojte všechna nepotřebná zařízení z počítače (například z adaptérů nebo docků).

**Pokud jste si nedávno nainstalovali aktualizaci na počítač, můžete si vrátit zpátky svůj ovladač zobrazení:**

1. Vyberte **Start**, zadejte **Správce zařízení**a z výsledků vyberte **Správce zařízení** .
2. Rozbalte oddíl Display Adapters ( **grafické adaptéry** ), klikněte pravým tlačítkem myši na grafický adaptér ANDS vyberte **vlastnosti**.
3. Přejděte na kartu **ovladač** a vyberte **vrátit změny ovladače**. <br>
Poznámka: Pokud tato možnost není dostupná nebo je zobrazená šedě, vyberte v možnostech níže možnost **ne** a přejděte tak k dalšímu kroku.
4. Aby se změny projevily, může být potřeba restartovat počítač.

**Odinstalace a přeinstalace ovladače zobrazení:**

1. Vyberte **Start**, zadejte **Správce zařízení**a z výsledků vyberte **Správce zařízení** .
2. Rozbalte oddíl Display Adapters ( **grafické adaptéry** ), klikněte pravým tlačítkem myši na grafický adaptér ANDS vyberte **odinstalovat zařízení**. 
3. Zaškrtněte políčko vedle **Odstranit software ovladače tohoto zařízení** a vyberte **odinstalovat**.<br>
Poznámka: můžete být požádáni o restartování počítače v této fázi. Než začnete, zapište si zbývající pokyny.
4. Spusťte znovu Správce zařízení.
5. Rozbalte oddíl Display Adapters ( **grafické adaptéry** ), klikněte pravým tlačítkem na grafický adaptér a vyberte **Aktualizovat ovladač**.
6. **Pro aktualizaci softwaru ovladače vyberte Hledat automaticky** a postupujte podle pokynů k instalaci.