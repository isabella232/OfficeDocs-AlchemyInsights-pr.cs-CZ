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
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="7ee78-102">Poradce při potížích s úlohou Služby importu</span><span class="sxs-lookup"><span data-stu-id="7ee78-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="7ee78-103">Pokud máte problémy s úlohami služby Import, které se zasekly nebo selhávají, zkontrolujte a vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="7ee78-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="7ee78-104">Zkontrolujte velikost souboru PST.</span><span class="sxs-lookup"><span data-stu-id="7ee78-104">Review the size of of the PST file.</span></span> <span data-ttu-id="7ee78-105">Maximální doporučená velikost souboru PST pro import je 20 GB.</span><span class="sxs-lookup"><span data-stu-id="7ee78-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="7ee78-106">Pokud máte podezření, že přeskočené položky kvůli poškození, spusťte Scanpst.exe diagnostikovat a opravit chyby v souborech PST.</span><span class="sxs-lookup"><span data-stu-id="7ee78-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="7ee78-107">Pokud se při importu zobrazí chyba "MapiExceptionShutoffQuotaExceeded", ujistěte se, že cílová poštovní schránka má dostatečnou kapacitu pro import požadovaných souborů PST.</span><span class="sxs-lookup"><span data-stu-id="7ee78-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="7ee78-108">Další informace o řešení problémů s úlohami importu pst najdete v tématu Řešení [problémů s úlohami importu pst](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="7ee78-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="7ee78-109">Informace o tom, jak vyřešit problémy při importu pstů do Outlook, najdete v článku Řešení problémů s importem souboru .pst Outlook [(microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="7ee78-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>