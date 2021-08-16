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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034747"
---
# <a name="fix-transport-rules"></a>Oprava pravidel přenosu

Tato zpráva se týká vlastního pravidla toku pošty. Pokud chcete zkontrolovat přesné pravidlo, proveďte toto:

1. Ve výsledcích odeslání si v části **Další informace** poznamenejte **identifikátor GUID** nebo název **zásady**.
2. Spusťte Exchange Management Shell. Další informace najdete v [tématu Otevření Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Spusťte tento příkaz (pomocí identifikátoru GUID z odeslání):  **Get-TransportRule -identity "GUID" | fl * Description***
4. V popisu se zobrazí nakonfigurované podmínky, které ovlivnily zprávu.

Další informace najdete v tématu [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
