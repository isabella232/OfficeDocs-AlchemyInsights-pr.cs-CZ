---
title: Poradce při potížích s zaregistrovat zařízení s Androidem v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708991"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="dc0b2-102">Poradce při potížích s zaregistrovat zařízení s Androidem v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="dc0b2-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="dc0b2-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="dc0b2-104">Některé běžné problémy a kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="dc0b2-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="dc0b2-105">**Chyba Šifrované zařízení na portálu společnosti:** Novější verze Androidu, konkrétně od verze 7.0, vyžadují přístupové heslo při spuštění, aby bylo vaše zařízení plně zašifrované.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="dc0b2-106">Běžnými řešeními je povolit připnutí při spuštění nebo plně zašifrovat zařízení.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="dc0b2-107">Další [informace najdete v](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="dc0b2-108">**Zařízení se nepodaří služby Intune** zkontrolovat nebo se v konzole pro správu Intune zobrazí jako není v pořádku: Některá zařízení Samsung 4.4 a 5.5 nemusí služby zkontrolovat.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="dc0b2-109">Existují 3 možná řešení tohoto problému:</span><span class="sxs-lookup"><span data-stu-id="dc0b2-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="dc0b2-110">Ručně otevřete aplikaci Portál společnosti Intune, která automaticky spustí synchronizaci zařízení.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="dc0b2-111">Aktualizujte zařízení na Android 6.0 nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="dc0b2-112">Zakažte Samsung Smart Manageru správu portálu společnosti Intune.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="dc0b2-113">Další [podrobnosti o těchto](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) problémech a řešeních najdete v tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="dc0b2-114">**Chyba typu Neplatná licence** nebo **Uživatelské jméno:** Uživatel musí mít přiřazenou licenci Intune nebo EMS.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="dc0b2-115">Tyto dokumenty si projdete a přiřadíte licenci prostřednictvím: Centra pro správu Office nebo portálu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="dc0b2-116">Další zdroje informací, které vám pomůžou problém vyřešit:</span><span class="sxs-lookup"><span data-stu-id="dc0b2-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="dc0b2-117">Pomocí [portálu Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby registrace.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="dc0b2-118">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="dc0b2-119">V [tomto dokumentu se](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) můžete se seznamem běžných chyb, které brání zápisu a řešení každého z nich.</span><span class="sxs-lookup"><span data-stu-id="dc0b2-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="dc0b2-120">[Zjistěte, jak zaregistrovat zařízení s Androidem v Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="dc0b2-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
