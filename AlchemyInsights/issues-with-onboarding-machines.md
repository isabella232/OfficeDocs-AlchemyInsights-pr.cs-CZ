---
title: Problémy s počítači s připojením k programu Microsoft Defender pro koncové body
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901560"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="f2274-102">Problémy s počítači s připojením k programu Microsoft Defender pro koncové body</span><span class="sxs-lookup"><span data-stu-id="f2274-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="f2274-103">Můžete mít problémy s připojením počítačů ke službě MDE.</span><span class="sxs-lookup"><span data-stu-id="f2274-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="f2274-104">Pokud máte přístup k počítači koncového uživatele, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="f2274-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="f2274-105">Stáhněte si nejnovější verzi Preview diagnostického [nástroje MDE Client Analyzer.](https://aka.ms/betamdeanalyzer)</span><span class="sxs-lookup"><span data-stu-id="f2274-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="f2274-106">Klikněte pravým **tlačítkem myši na MDEClientAnalyzer.cmd** a vyberte Spustit jako správce.</span><span class="sxs-lookup"><span data-stu-id="f2274-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="f2274-107">Postupujte podle pokynů navrhovaných v **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="f2274-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="f2274-108">Podrobnější protokoly najdete v vytvořené podsadě s názvem **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="f2274-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="f2274-109">Pokud potřebujete další pokyny, kontaktujte [podporu Microsoft Defenderu pro](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) koncový bod a poskytnte výsledný MDEClientAnalyzerResult.zip soubor pro analýzu.</span><span class="sxs-lookup"><span data-stu-id="f2274-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
