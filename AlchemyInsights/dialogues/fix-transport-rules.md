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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693296"
---
# <a name="fix-transport-rules"></a>Oprava pravidel přenosu

Tuto zprávu ovlivnilo vlastní pravidlo toku pošty. Když chcete zkontrolovat přesné pravidlo, proveďte toto:

1. Ve výsledcích odeslání si v části **Další informace** poznamenejte **identifikátor GUID** nebo **název zásady.**
2. Spusťte prostředí Exchange Management Shell. Další informace najdete v článku [o otevření prostředí Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Spusťte tento příkaz (pomocí identifikátoru GUID pro odeslání):  **Get-TransportRule -identity "GUID" | fl * Popis***
4. Prohlédněte si popis a podívejte se na nakonfigurované podmínky, které zprávu ovlivnily.

Další informace najdete v [tématu Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
