---
title: Poradce při potížích s registraci zařízení s iOSem v Microsoft Intune
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708955"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e353b-102">Poradce při potížích s registraci zařízení s iOSem v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e353b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e353b-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="e353b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e353b-104">Některé běžné chybové zprávy a kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="e353b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e353b-105">**Dosáhli jste limitu zařízení** Uživatel má zaregistrované víc zařízení, než je limit počtu zařízení.</span><span class="sxs-lookup"><span data-stu-id="e353b-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e353b-106">V těchto dokumentech můžete [odebrat zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) změnit limit [zařízení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="e353b-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e353b-107">**Tato služba není podporovaná. Žádné zásady registrace: Služba** nabízených oznámení Apple (APNS) se musí nakonfigurovat nebo prodloužit.</span><span class="sxs-lookup"><span data-stu-id="e353b-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e353b-108">Pokyny [k tomu najdete](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) v tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="e353b-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e353b-109">**Neplatný typ uživatelské licence nebo uživatelské jméno není rozpoznáno:** Uživatel musí mít přiřazenou licenci k Intune nebo EMS.</span><span class="sxs-lookup"><span data-stu-id="e353b-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e353b-110">Tyto dokumenty si projdete a přiřadíte licenci prostřednictvím: [Centra pro správu Office](https://docs.microsoft.com/intune/licenses-assign) nebo portálu Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="e353b-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e353b-111">Další zdroje informací, které vám pomůžou problém vyřešit:</span><span class="sxs-lookup"><span data-stu-id="e353b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e353b-112">Pomocí [portálu Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby registrace.</span><span class="sxs-lookup"><span data-stu-id="e353b-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e353b-113">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="e353b-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e353b-114">V těchto dokumentech najdete seznam běžných chyb, které zabraňují jejich zápisu a [řešení:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Průvodce odstraňováním potíží a [Řešení potíží s dokumentem.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="e353b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e353b-115">[Zjistěte, jak zaregistrovat zařízení s iOSem v Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="e353b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

