---
title: Problémy s vestavěnými počítači
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676875"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="99cd9-102">Problémy s vestavěnými počítači</span><span class="sxs-lookup"><span data-stu-id="99cd9-102">Issues with onboarding machines</span></span>

<span data-ttu-id="99cd9-103">Je možné, že máte problémy s MDATP službami.</span><span class="sxs-lookup"><span data-stu-id="99cd9-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="99cd9-104">Pokud máte přístup k počítači s koncovým uživatelem, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="99cd9-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="99cd9-105">Stáhněte diagnostický nástroj [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="99cd9-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="99cd9-106">Extrahujte a spusťte MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="99cd9-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="99cd9-107">Vyhledejte diagnostický protokol ve složce s názvem MDATPClientAnalyzerResult, což je stejná složka, ve které je nástroj Analyzer stažen.</span><span class="sxs-lookup"><span data-stu-id="99cd9-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="99cd9-108">Zkontrolujte soubor protokolu, MDATPClientAnalyzer.txt a najděte problémy s nastavením připojení nebo proxy serveru pro Internet.</span><span class="sxs-lookup"><span data-stu-id="99cd9-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>