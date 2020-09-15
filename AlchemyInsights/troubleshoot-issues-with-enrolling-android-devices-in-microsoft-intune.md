---
title: Poradce při potížích s registrací zařízení s Androidem v Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689947"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="a5068-102">Poradce při potížích s registrací zařízení s Androidem v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a5068-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="a5068-103">Prohlédněte si níže uvedené zdroje a problém vyřešte.</span><span class="sxs-lookup"><span data-stu-id="a5068-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a5068-104">Některé běžné problémy a řešení:</span><span class="sxs-lookup"><span data-stu-id="a5068-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="a5068-105">**Chyba nešifrovaného zařízení na portálu společnosti:** Novější verze Androidu, zejména od verze 7.0, vyžadují spouštěcí heslo, abyste měli jistotu, že vaše zařízení je plně šifrované.</span><span class="sxs-lookup"><span data-stu-id="a5068-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="a5068-106">Běžná řešení: Povolte spouštěcí PIN nebo plně Zašifrujte zařízení.</span><span class="sxs-lookup"><span data-stu-id="a5068-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="a5068-107">V [tomto dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) najdete další informace.</span><span class="sxs-lookup"><span data-stu-id="a5068-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="a5068-108">Zařízení se nepovedlo **vrátit se změnami a zobrazit jako "v nesprávném stavu" v konzoli správce Intune:** Některá zařízení Samsung 4,4 a 5,5 nemusí tuto službu vrátit.</span><span class="sxs-lookup"><span data-stu-id="a5068-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="a5068-109">Existuje 3 možná řešení tohoto problému:</span><span class="sxs-lookup"><span data-stu-id="a5068-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="a5068-110">Ručně otevřete aplikaci Portál společnosti Intune, která automaticky zahájí synchronizaci zařízení.</span><span class="sxs-lookup"><span data-stu-id="a5068-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="a5068-111">Aktualizujte zařízení na Android 6,0 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="a5068-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="a5068-112">Zakažte čipovou kartu Samsung pro správu portálu společnosti Intune.</span><span class="sxs-lookup"><span data-stu-id="a5068-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="a5068-113">V [tomto dokumentu](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) najdete další podrobnosti o těchto problémech a řešeních.</span><span class="sxs-lookup"><span data-stu-id="a5068-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="a5068-114">**Typ uživatelské licence není platný** nebo **došlo k neznámé chybě uživatelského jména:** uživateli musí být přiřazena licence Intune nebo EMS.</span><span class="sxs-lookup"><span data-stu-id="a5068-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="a5068-115">V těchto dokumentech si můžete přiřadit licenci pomocí centra pro správu Office nebo Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="a5068-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="a5068-116">Další zdroje informací pro řešení vašeho problému:</span><span class="sxs-lookup"><span data-stu-id="a5068-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a5068-117">Na [portálu Poradce při potížích s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby zápisu.</span><span class="sxs-lookup"><span data-stu-id="a5068-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a5068-118">Další podrobnosti najdete v [tomto dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="a5068-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="a5068-119">V [tomto dokumentu](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) se zobrazí seznam běžných chyb, které se zabrání zápisu a řešení každého z nich.</span><span class="sxs-lookup"><span data-stu-id="a5068-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="a5068-120">[Naučte se zapisovat zařízení s Androidem v Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="a5068-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
