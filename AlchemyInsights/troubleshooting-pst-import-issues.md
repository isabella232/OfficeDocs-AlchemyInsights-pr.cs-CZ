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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="bcae9-102">Řešení potíží s importem souborů PST</span><span class="sxs-lookup"><span data-stu-id="bcae9-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="bcae9-103">Pokud importujete v samotném klientovi Outlooku, podívejte se na řešení problémů [s importem souboru .pst Outlooku.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="bcae9-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="bcae9-104">Pokud používáte Službu importu a je zaseknutá, nezapomeňte, že každý soubor PST, který nahrajete do umístění Azure Storage, by neměl být větší než 20 GB.</span><span class="sxs-lookup"><span data-stu-id="bcae9-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="bcae9-105">Soubory PST větší než 20 GB mohou mít vliv na výkon procesu importu pst.</span><span class="sxs-lookup"><span data-stu-id="bcae9-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="bcae9-106">Další informace o řešení potíží s uvíznutými úlohami najdete v tématu [Problémy, které mají vliv na úlohy importu ve formátu PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="bcae9-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="bcae9-107">Pokud chcete ověřit stav konkrétní úlohy importu, použijte [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="bcae9-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="bcae9-108">Úplné podrobnosti o službě importu najdete v tématu Přehled importu souborů [PST vaší organizace.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="bcae9-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
