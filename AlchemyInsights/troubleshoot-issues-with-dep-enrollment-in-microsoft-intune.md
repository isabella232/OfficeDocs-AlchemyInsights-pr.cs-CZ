---
title: Řešení problémů s registrací funkce Zabránění spuštění dat v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 27abeafba5588ca74569ba6bebc5d940b767ea3f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824500"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="76e20-102">Řešení problémů s registrací funkce Zabránění spuštění dat v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="76e20-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="76e20-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="76e20-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="76e20-104">Pokud se zařízení DEP nedaří zaregistrovat a je povolené vícefaktorové ověřování (MFA), zakažte MFA.</span><span class="sxs-lookup"><span data-stu-id="76e20-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="76e20-105">V současné době není pro zápis funkce Zabránění spuštění dat podporována MFA.</span><span class="sxs-lookup"><span data-stu-id="76e20-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="76e20-106">K [diagnostice a](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) řešení běžných chyb registrace použijte Portál řešení potíží s Intune.</span><span class="sxs-lookup"><span data-stu-id="76e20-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="76e20-107">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="76e20-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="76e20-108">V těchto dokumentech najdete seznam běžných chyb, které brání zápisu a řešení jednotlivých [dokumentů:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Průvodce odstraňováním potíží a [Dokument pro řešení potíží.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="76e20-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="76e20-109">[Přečtěte si o programu registrace zařízení.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="76e20-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
