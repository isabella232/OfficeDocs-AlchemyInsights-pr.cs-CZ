---
title: Nástroj pro export eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711088"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nejde nainstalovat nebo spustit nástroj pro export eDiscovery?

Pokud se vám nedaří nainstalovat nebo spustit nástroj pro export eDiscovery ke stažení výsledků hledání, podívejte se na tyto věci:
  
- Počítač, který používáte, splňuje tyto předpoklady:

  - 32 nebo 64 verze Windows 7 a novější verze

  - Microsoft .NET Framework 4.7

  - Podporovaný prohlížeč:

  - Microsoft Edge

    Nebo

  - Internet Explorer 10 a novější verze

    Jiné prohlížeče, například Google Chrome a Mozilla Firefox, nejsou podporované.

- Vaše organizace se může připojit ke koncovému bodu v Azure, což je ** \* . blob.Core.Windows.NET** (zástupný znak představuje jedinečný identifikátor úlohy exportu).

- Přiřadili jste roli exportu v centru zabezpečení Microsoft 365 &amp; . Ve výchozím nastavení je tato role přiřazena jenom skupině role správce eDiscovery. Viz [přiřazení oprávnění eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Další informace najdete v článku [Export výsledků hledání obsahu](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  