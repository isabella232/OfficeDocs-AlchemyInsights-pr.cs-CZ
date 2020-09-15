---
title: Poradce při potížích s registrací zařízení iOS v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669241"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="32c79-102">Poradce při potížích s registrací zařízení iOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="32c79-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="32c79-103">Prohlédněte si níže uvedené zdroje a problém vyřešte.</span><span class="sxs-lookup"><span data-stu-id="32c79-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="32c79-104">Některé běžné chybové zprávy a postupy řešení:</span><span class="sxs-lookup"><span data-stu-id="32c79-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="32c79-105">**Zakončení zařízení** Uživatel má více popsaných zařízení, než je limit zařízení.</span><span class="sxs-lookup"><span data-stu-id="32c79-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="32c79-106">Pokud chcete [Odebrat zařízení](https://docs.microsoft.com/intune/devices-wipe) nebo [změnit limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), Projděte si tyto dokumenty.</span><span class="sxs-lookup"><span data-stu-id="32c79-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="32c79-107">**Tato služba není podporovaná. Žádné zásady zápisu:** službu APNs (Apple Push Notification Service) je třeba nakonfigurovat nebo obnovit.</span><span class="sxs-lookup"><span data-stu-id="32c79-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="32c79-108">V [tomto dokumentu](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) najdete pokyny, jak to udělat.</span><span class="sxs-lookup"><span data-stu-id="32c79-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="32c79-109">**Typ uživatelské licence není platný nebo nejde rozpoznat uživatelské jméno:** Uživateli musí být přiřazena licence Intune nebo EMS.</span><span class="sxs-lookup"><span data-stu-id="32c79-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="32c79-110">V těchto dokumentech si můžete přiřadit licenci pomocí [centra pro správu Office](https://docs.microsoft.com/intune/licenses-assign) nebo [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="32c79-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="32c79-111">Další zdroje informací pro řešení vašeho problému:</span><span class="sxs-lookup"><span data-stu-id="32c79-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="32c79-112">Na [portálu Poradce při potížích s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby zápisu.</span><span class="sxs-lookup"><span data-stu-id="32c79-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="32c79-113">Další podrobnosti najdete v [tomto dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="32c79-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="32c79-114">V těchto dokumentech se podívejte na seznam běžných chyb, které zabraňují zápisu a řešení každého z nich: [Poradce při potížích](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [odstraňování potíží s dokumentem](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="32c79-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="32c79-115">[Naučte se zapisovat zařízení s iOS v Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="32c79-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

