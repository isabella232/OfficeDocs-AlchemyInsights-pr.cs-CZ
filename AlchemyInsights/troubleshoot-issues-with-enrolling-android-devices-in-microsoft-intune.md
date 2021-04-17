---
title: Řešení problémů s registracemi zařízení s Androidem v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830935"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d5a04-102">Řešení problémů s registracemi zařízení s Androidem v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d5a04-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d5a04-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="d5a04-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d5a04-104">Některé běžné problémy a kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="d5a04-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d5a04-105">**Chyba zařízení není šifrovaná na portálu společnosti:** Novější verze Androidu, zejména od verze 7.0, vyžadují spouštěcí heslo, aby bylo zařízení plně zašifrované.</span><span class="sxs-lookup"><span data-stu-id="d5a04-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d5a04-106">Běžnými řešeními je povolit připnutí při spuštění nebo plně zašifrovat zařízení.</span><span class="sxs-lookup"><span data-stu-id="d5a04-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d5a04-107">Další [informace najdete v tomto](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dokumentu.</span><span class="sxs-lookup"><span data-stu-id="d5a04-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d5a04-108">**Zařízení se nedaří se službou Intune** zkontrolovat nebo se v konzole pro správu Intune nezobrazovat jako "Není v pořádku": Některá zařízení Samsung 4.4 a 5.5 nemusí službu zkontrolovat.</span><span class="sxs-lookup"><span data-stu-id="d5a04-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d5a04-109">Existují 3 možná řešení tohoto problému:</span><span class="sxs-lookup"><span data-stu-id="d5a04-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d5a04-110">Ručně otevřete aplikaci Portál společnosti Intune, která automaticky zahájí synchronizaci zařízení.</span><span class="sxs-lookup"><span data-stu-id="d5a04-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d5a04-111">Aktualizujte zařízení na Android 6.0 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="d5a04-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d5a04-112">Zakažte Samsung Smart Manageru ve správě portálu společnosti Intune.</span><span class="sxs-lookup"><span data-stu-id="d5a04-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d5a04-113">Další [podrobnosti o těchto](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) problémech a řešeních najdete v tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="d5a04-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d5a04-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span><span class="sxs-lookup"><span data-stu-id="d5a04-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d5a04-115">Projděte si tyto dokumenty a přiřaďte licenci prostřednictvím: Centra pro správu Office nebo portálu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d5a04-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d5a04-116">Další zdroje informací, které vám pomůžou problém vyřešit:</span><span class="sxs-lookup"><span data-stu-id="d5a04-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d5a04-117">K [diagnostice a](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) řešení běžných chyb registrace použijte Portál řešení potíží s Intune.</span><span class="sxs-lookup"><span data-stu-id="d5a04-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d5a04-118">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="d5a04-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d5a04-119">V [tomto dokumentu se](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) můžete se seznamem běžných chyb, které brání zápisu a jejich řešení.</span><span class="sxs-lookup"><span data-stu-id="d5a04-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d5a04-120">[Zjistěte, jak zaregistrovat zařízení s Androidem v Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="d5a04-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
