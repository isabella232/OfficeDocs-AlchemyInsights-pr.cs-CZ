---
title: Problémy s palubními stroji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141364"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="7d217-102">Problémy s palubními stroji</span><span class="sxs-lookup"><span data-stu-id="7d217-102">Issues with onboarding machines</span></span>

<span data-ttu-id="7d217-103">Můžete mít problémy s onboarding počítače služby MDATP.</span><span class="sxs-lookup"><span data-stu-id="7d217-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="7d217-104">Pokud máte přístup k počítači koncového uživatele, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="7d217-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="7d217-105">Stáhněte si diagnostický nástroj [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="7d217-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="7d217-106">Extrahujte a spusťte soubor MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="7d217-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="7d217-107">Vyhledejte diagnostický protokol ve složce s názvem MDATPClientAnalyzerResult, stejné složce, do které se stahuje nástroj Analyzer.</span><span class="sxs-lookup"><span data-stu-id="7d217-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="7d217-108">Zkontrolujte soubor protokolu, MDATPClientAnalyzer.txt, abyste našli problémy s připojením nebo nastavením internetového proxy serveru.</span><span class="sxs-lookup"><span data-stu-id="7d217-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>