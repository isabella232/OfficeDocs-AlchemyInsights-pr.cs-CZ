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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059808"
---
# <a name="troubleshooting-pst-import-issues"></a>Řešení potíží s importem souborů PST

- Pokud importujete v samotném klientovi Outlooku, podívejte se na řešení problémů [s importem souboru .pst Outlooku.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Pokud používáte Službu importu a je zaseknutá, nezapomeňte, že každý soubor PST, který nahrajete do umístění Azure Storage, by neměl být větší než 20 GB. Soubory PST větší než 20 GB mohou mít vliv na výkon procesu importu pst. Další informace o řešení potíží s uvíznutými úlohami najdete v tématu [Problémy, které mají vliv na úlohy importu ve formátu PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Pokud chcete ověřit stav konkrétní úlohy importu, použijte [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Úplné podrobnosti o službě importu najdete v tématu Přehled importu souborů [PST vaší organizace.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
