---
title: Řešení potíží s importem souborů PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826156"
---
# <a name="troubleshooting-pst-import-issues"></a>Řešení potíží s importem souborů PST

- Pokud provádíte import přímo v klientovi Outlooku, podívejte se na článek o [řešení problémů s importem souboru .pst aplikace Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Pokud používáte Importovací službu a služba je zablokovaná, upozorňujeme, že žádný soubor PST, který budete odesílat do úložiště Azure, by neměl být větší než 20 GB. Soubory PST větší než 20 GB můžou mít vliv na výkon procesu importu souborů PST.

- Pokud chcete ověřit stav konkrétní úlohy importu, můžete použít příkaz [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Podrobné informace o importovací službě najdete v článku s [přehledem importu souborů PST vaší organizace](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
