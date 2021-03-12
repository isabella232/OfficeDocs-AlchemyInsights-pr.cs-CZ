---
title: Oprava pravidel přenosu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744843"
---
# <a name="fix-transport-rules"></a>Oprava pravidel přenosu

Tato zpráva se týká vlastního pravidla toku pošty. Pokud chcete zkontrolovat přesné pravidlo, proveďte toto:

1. Ve výsledcích odeslání si v části **Další informace** poznamenejte **identifikátor GUID** nebo název **zásady**.
2. Spusťte Prostředí Exchange Management Shell. Další informace najdete v tématu [Otevření prostředí Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Spusťte tento příkaz (pomocí identifikátoru GUID z odeslání):  **Get-TransportRule -identity "GUID" | fl * Description***
4. V popisu se zobrazí nakonfigurované podmínky, které ovlivnily zprávu.

Další informace najdete v tématu [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
