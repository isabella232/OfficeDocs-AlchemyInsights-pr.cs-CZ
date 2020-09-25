---
title: 1490 – řešení potíží – eDiscovery – chyby
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277835"
---
# <a name="troubleshoot-content-search-errors"></a>Řešení chyb při hledání obsahu

Máte problémy s vyhledáváním obsahu nebo se selháním při exportu výsledků hledání?

Při provádění hledání se například zobrazuje následující:

- Chyby CS008 nebo CS012

- Chyby při obsazení nebo vypršení časového limitu serveru

- Došlo k chybě aplikace.

Nebo při vyhledávání nebo exportu výsledků z velkého počtu poštovních schránek (přes 100 000 poštovních schránek) se zobrazují chyby při exportu?

U těchto typů chyb opakujte hledání u neúspěšných umístění obsahu. Další informace najdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Pokud exportujete víc než 100K poštovních schránek, budete muset ke stažení výsledků exportu použít následující PowerShell:  [Export výsledků z víc než 100K poštovní schránky](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
