---
title: Poradce při potížích s registrací zabránění spuštění dat v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708703"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="28438-102">Poradce při potížích s registrací zabránění spuštění dat v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="28438-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="28438-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="28438-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="28438-104">Pokud se zařízení zabránění spuštění dat nemůže zaregistrovat a je povolené vícefaktorové ověřování (MFA), zakažte prosím MFA.</span><span class="sxs-lookup"><span data-stu-id="28438-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="28438-105">Registrace zabránění spuštění dat v současné době nepodporuje MFA.</span><span class="sxs-lookup"><span data-stu-id="28438-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="28438-106">Pomocí [portálu Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby registrace.</span><span class="sxs-lookup"><span data-stu-id="28438-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="28438-107">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="28438-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="28438-108">Seznam běžných chyb, které brání zápisu a řešení problémů s jednotlivými, najdete v těchto [dokumentech:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Průvodce odstraňováním potíží a Řešení potíží s [dokumentem](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="28438-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="28438-109">[Přečtěte si informace o programu pro registraci zařízení.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="28438-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
