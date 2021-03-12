---
title: Vzdáleně opravte problémy s připojením zařízení s Windows 10 do programu Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744722"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="a1002-102">Vzdáleně opravte problémy s připojením zařízení s Windows 10 do programu Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a1002-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="a1002-103">Pokud máte přístup ke vzdálenému počítači, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="a1002-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="a1002-104">Stáhněte si diagnostický nástroj [Client Connectivity Analyzer.](https://go.microsoft.com/fwlink/?linkid=2143466)</span><span class="sxs-lookup"><span data-stu-id="a1002-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="a1002-105">Extrahujte a spusťte MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="a1002-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="a1002-106">Vyhledejte diagnostický protokol ve složce MDATPClientAnalyzerResult, což je stejná složka, ve které byl nástroj Analyzer stažen.</span><span class="sxs-lookup"><span data-stu-id="a1002-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="a1002-107">Pokud chcete najít problémy s připojením nebo nastavením internetového proxy serveru, zkontrolujte soubor protokolu MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="a1002-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="a1002-108">Další informace najdete v tématu Problémy s počítači s [připojením.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="a1002-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
