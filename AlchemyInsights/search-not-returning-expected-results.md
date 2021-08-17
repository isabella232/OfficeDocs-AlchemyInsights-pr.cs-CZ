---
title: 1491-search-not-return-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052703"
---
# <a name="content-search-not-returning-expected-results"></a>Hledání obsahu nevrací očekávané výsledky

Při spuštění vyhledávání obsahu z centra Microsoft 365 zabezpečení & dodržování předpisů se vám mohou zobrazit neočekávané výsledky hledání. Zvažte následující věci, které mohou mít vliv na výsledky hledání:

- Umístění obsahu a **podmínky hledání:** Ujistěte se, že jste vybrali správná umístění obsahu a podmínky hledání. Pokud jste spustili velké hledání (s mnoha místy), zvažte jeho rozdělení do několika hledání.

- **Částečně indexované položky:**  [Částečně indexované položky](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z poštovních schránek jsou zahrnuté do předpokládaných výsledků hledání. Částečně indexované položky z webů v SharePoint OneDrive ale nejsou zahrnuté do odhadu hledání.

- Chyby **hledání:** Při hledání velkého počtu poštovních schránek (přes 100 000 poštovních schránek) se mohou zobrazit chyby hledání s kódy chyb, jako jsou NAPŘÍKLAD CS008-009 a CS012-002). V takovém případě zkuste hledání opakovat jenom pro umístění obsahu, která selhala. Další  [informace najdete v](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) tomto článku.
