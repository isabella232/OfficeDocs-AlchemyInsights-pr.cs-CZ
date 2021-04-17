---
title: Řešení problémů s registracemi zařízení s iOSem v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823456"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="62bf3-102">Řešení problémů s registracemi zařízení s iOSem v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="62bf3-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="62bf3-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="62bf3-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="62bf3-104">Některé běžné chybové zprávy a kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="62bf3-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="62bf3-105">**Bylo dosaženo krytu zařízení** Uživatel má zaregistrovaná víc zařízení, než je limit zařízení.</span><span class="sxs-lookup"><span data-stu-id="62bf3-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="62bf3-106">Zkontrolujte tyto dokumenty a [odeberte zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) [změňte limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="62bf3-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="62bf3-107">**Tato služba není podporovaná. Žádné zásady registrace:** Služba APNS (Apple Push Notification Service) musí být nakonfigurovaná nebo obnovená.</span><span class="sxs-lookup"><span data-stu-id="62bf3-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="62bf3-108">Pokyny [k tomu najdete](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) v tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="62bf3-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="62bf3-109">**Typ uživatelské licence: Neplatné nebo Uživatelské jméno není rozpoznáno:** Uživateli je potřeba přiřadit licenci Intune nebo EMS.</span><span class="sxs-lookup"><span data-stu-id="62bf3-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="62bf3-110">Projděte si tyto dokumenty a přiřaďte licenci prostřednictvím: [Centra pro](https://docs.microsoft.com/intune/licenses-assign) správu Office nebo portálu [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="62bf3-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="62bf3-111">Další zdroje informací, které vám pomůžou problém vyřešit:</span><span class="sxs-lookup"><span data-stu-id="62bf3-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="62bf3-112">K [diagnostice a](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) řešení běžných chyb registrace použijte Portál řešení potíží s Intune.</span><span class="sxs-lookup"><span data-stu-id="62bf3-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="62bf3-113">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="62bf3-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="62bf3-114">V těchto dokumentech najdete seznam běžných chyb, které brání zápisu a řešení jednotlivých dokumentů: [Průvodce](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) odstraňováním potíží a [Poradce při potížích s dokumentem](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="62bf3-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="62bf3-115">[Zjistěte, jak zaregistrovat zařízení s iOSem v Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="62bf3-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

