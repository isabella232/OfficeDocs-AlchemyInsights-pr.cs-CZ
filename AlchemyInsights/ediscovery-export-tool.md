---
title: Nástroj pro export eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101295"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nemůžete nainstalovat nebo spustit nástroj pro export eDiscovery?

Pokud nemůžete nainstalovat nebo spustit nástroj pro export eDiscovery a stáhnout výsledky hledání, podívejte se na následující věci:
  
- Počítač, který používáte, splňuje tyto předpoklady:

  - 32bitová nebo 64bitová verze Windows 7 a novějších verzích

  - Microsoft .NET Framework 4.7

  - Podporovaný prohlížeč:

  - Microsoft Edge

    Nebo

  - Internet Explorer 10 a novějších verzích

    Jiné prohlížeče, jako je Google Chrome nebo Mozilla Firefox, nejsou podporované.

- Vaše organizace se může připojit k koncovému bodu v Azure, což je **\* .blob.core.windows.net** (zástupný znak představuje jedinečný identifikátor exportu).

- V Centru dodržování předpisů zabezpečení se vám přiřadí role Export Microsoft 365 &amp; zabezpečení. Ve výchozím nastavení je tato role přiřazená jenom skupině rolí Správce eDiscovery. Viz [Přiřazení oprávnění k eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Další informace najdete v článku [Export výsledků hledání obsahu](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Pokud exportujete víc než 100 tisíc poštovních schránek, budete muset stáhnout výsledky exportu pomocí následujícího PowerShellu: Export výsledků z více než  [100 tisíc poštovních schránek](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).