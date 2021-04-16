---
title: Řešení problémů s registracemi zařízení s Windows v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808964"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="8a17f-102">Řešení problémů s registracemi zařízení s Windows v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8a17f-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="8a17f-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="8a17f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="8a17f-104">Některé běžné chybové zprávy a kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="8a17f-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="8a17f-105">**Software nelze nainstalovat, 0x80cf4017:** Platnost certifikátu vašeho účtu vypršela.</span><span class="sxs-lookup"><span data-stu-id="8a17f-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="8a17f-106">Znovu stáhněte softwarový balíček Klienta počítače v konzole pro správu Intune.</span><span class="sxs-lookup"><span data-stu-id="8a17f-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="8a17f-107">Další informace najdete v této dokumentaci.</span><span class="sxs-lookup"><span data-stu-id="8a17f-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="8a17f-108">**Kód chyby 0x801c0003:** K chybě může dojít v následujících situacích:</span><span class="sxs-lookup"><span data-stu-id="8a17f-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="8a17f-109">Uživatel má zaregistrovaná víc zařízení, než je limit zařízení.</span><span class="sxs-lookup"><span data-stu-id="8a17f-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8a17f-110">Zkontrolujte tyto dokumenty a [odeberte zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) [změňte limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="8a17f-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="8a17f-111">"Uživatelé se smí připojit k Azure AD" je nastavené na "žádné".</span><span class="sxs-lookup"><span data-stu-id="8a17f-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="8a17f-112">Nastavte ho na všechny nebo vyberte uživatele.</span><span class="sxs-lookup"><span data-stu-id="8a17f-112">Set it to all or select users.</span></span> <span data-ttu-id="8a17f-113">Další [informace najdete v](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) této dokumentaci.</span><span class="sxs-lookup"><span data-stu-id="8a17f-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="8a17f-114">Zařízení už zaregistroval jiný uživatel.</span><span class="sxs-lookup"><span data-stu-id="8a17f-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="8a17f-115">V takovém případě odeberte zařízení z konzoly Azure Intune nebo zařízení před znova ručně derollujte.</span><span class="sxs-lookup"><span data-stu-id="8a17f-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="8a17f-116">Zařízení je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="8a17f-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="8a17f-117">K Azure Active Directory se mohou připojit jenom windows 10 Pro, education a podnikové skladové skladové organizace.</span><span class="sxs-lookup"><span data-stu-id="8a17f-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="8a17f-118">Další zdroje informací, které vám pomůžou problém vyřešit:</span><span class="sxs-lookup"><span data-stu-id="8a17f-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="8a17f-119">K [diagnostice a](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) řešení běžných chyb registrace použijte Portál řešení potíží s Intune.</span><span class="sxs-lookup"><span data-stu-id="8a17f-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8a17f-120">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="8a17f-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="8a17f-121">V těchto dokumentech najdete seznam běžných chyb, které brání zápisu a řešení jednotlivých dokumentů: [Průvodce](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) odstraňováním potíží a [Poradce při potížích s dokumentem](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8a17f-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="8a17f-122">[Zjistěte, jak zaregistrovat zařízení s Windows v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="8a17f-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
