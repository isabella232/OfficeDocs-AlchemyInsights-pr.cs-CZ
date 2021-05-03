---
title: Poradce při potížích s úlohou Služby importu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "52124916"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Poradce při potížích s úlohou Služby importu

Pokud máte problémy s úlohami služby Import, které se zasekly nebo selhávají, zkontrolujte a vyzkoušejte následující postup:

- Zkontrolujte velikost souboru PST. Maximální doporučená velikost souboru PST pro import je 20 GB.

- Pokud máte podezření, že přeskočené položky kvůli poškození, spusťte Scanpst.exe diagnostikovat a opravit chyby v souborech PST.

- Pokud se při importu zobrazí chyba "MapiExceptionShutoffQuotaExceeded", ujistěte se, že cílová poštovní schránka má dostatečnou kapacitu pro import požadovaných souborů PST.

Další informace o řešení problémů s úlohami importu pst najdete v tématu Řešení [problémů s úlohami importu pst](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Informace o tom, jak vyřešit problémy při importu pstů do Outlook, najdete v článku Řešení problémů s importem souboru .pst Outlook [(microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).