---
title: 1491 – hledání – nevracení – očekávané – výsledky
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740467"
---
# <a name="content-search-not-returning-expected-results"></a>Hledání obsahu nevrací očekávané výsledky

Když spouštíte hledání obsahu z centra zabezpečení Microsoft 365 Security &, může se zobrazit neočekávané výsledky hledání. Zvažte následující věci, které můžou mít vliv na výsledky hledání:

- **Umístění obsahu a podmínky vyhledávání**: Ujistěte se, že jste vybrali správná umístění obsahu a podmínky vyhledávání. Pokud jste spustili velké vyhledávání (s mnoha umístěními), zvažte možnost rozdělení do několika hledání.

- **Částečně indexované položky**:  [částečně indexované položky](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z poštovních schránek se zahrnují do odhadovaných výsledků hledání. Částečně indexované položky z webů v SharePointu a OneDrivu se ale do odhadu hledání nezahrnují.

- **Neúspěšné hledání**: při hledání velkého počtu poštovních schránek (přes 100 000 poštovních schránek) se můžou zobrazit chyby hledání pomocí kódů chyb, jako je CS008-009 a CS012-002). V tomto případě opakujte hledání pouze pro umístění s neúspěšným obsahem. Další informace najdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
