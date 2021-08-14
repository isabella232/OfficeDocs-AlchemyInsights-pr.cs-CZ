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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972412"
---
# <a name="troubleshooting-pst-import-issues"></a>Řešení potíží s importem souborů PST

- Pokud importujete v rámci samotného klienta Outlook, podívejte se na řešení problémů s [importem Outlook .pst](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Pokud používáte Službu importu a je zaseknutá, nezapomeňte, že každý soubor PST, který nahrajete do Azure Storage umístění, by neměl být větší než 20 GB. Soubory PST větší než 20 GB mohou mít vliv na výkon procesu importu pst. Další informace o řešení potíží s uvíznutými úlohami najdete v tématu [Problémy, které mají vliv na úlohy importu ve formátu PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Pokud chcete ověřit stav konkrétní úlohy importu, použijte [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Úplné podrobnosti o službě importu najdete v tématu Přehled importu souborů [PST vaší organizace.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
