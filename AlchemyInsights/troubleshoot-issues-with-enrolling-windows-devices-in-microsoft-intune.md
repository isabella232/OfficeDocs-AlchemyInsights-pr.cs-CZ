---
title: Poradce při potížích s registraci zařízení s Windows v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708883"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="e588e-102">Poradce při potížích s registraci zařízení s Windows v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e588e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="e588e-103">Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.</span><span class="sxs-lookup"><span data-stu-id="e588e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e588e-104">Některé běžné chybové zprávy a kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="e588e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="e588e-105">**Software nelze nainstalovat, 0x80cf4017:** Platnost certifikátu účtu vypršela.</span><span class="sxs-lookup"><span data-stu-id="e588e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="e588e-106">V konzole pro správu Intune znovu stáhněte softwarový balíček Klienta počítače.</span><span class="sxs-lookup"><span data-stu-id="e588e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="e588e-107">Další informace najdete v této dokumentaci.</span><span class="sxs-lookup"><span data-stu-id="e588e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="e588e-108">**Kód chyby 0x801c0003:** K chybě může dojít v následujících situacích:</span><span class="sxs-lookup"><span data-stu-id="e588e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="e588e-109">Uživatel má zaregistrované víc zařízení, než je limit počtu zařízení.</span><span class="sxs-lookup"><span data-stu-id="e588e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e588e-110">V těchto dokumentech můžete [odebrat zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) změnit limit [zařízení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="e588e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="e588e-111">Možnost "Uživatelé mohou připojit zařízení k Azure AD" je nastavena na hodnotu "žádný".</span><span class="sxs-lookup"><span data-stu-id="e588e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="e588e-112">Nastavte ji na všechny uživatele nebo vyberte uživatele.</span><span class="sxs-lookup"><span data-stu-id="e588e-112">Set it to all or select users.</span></span> <span data-ttu-id="e588e-113">Další [informace najdete v](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) této dokumentaci.</span><span class="sxs-lookup"><span data-stu-id="e588e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="e588e-114">Zařízení už zaregistroval jiný uživatel.</span><span class="sxs-lookup"><span data-stu-id="e588e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="e588e-115">V takovém případě odeberte zařízení z konzoly Azure Intune nebo ho před pokusem znovu ručně derollujte.</span><span class="sxs-lookup"><span data-stu-id="e588e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="e588e-116">Zařízení je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="e588e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="e588e-117">K Azure Active Directory se může připojit jenom skladové soubory Windows 10 Pro, Education a Enterprise.</span><span class="sxs-lookup"><span data-stu-id="e588e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="e588e-118">Další zdroje informací, které vám pomůžou problém vyřešit:</span><span class="sxs-lookup"><span data-stu-id="e588e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="e588e-119">Pomocí [portálu Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby registrace.</span><span class="sxs-lookup"><span data-stu-id="e588e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e588e-120">Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.</span><span class="sxs-lookup"><span data-stu-id="e588e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="e588e-121">V těchto dokumentech najdete seznam běžných chyb, které zabraňují jejich zápisu a [řešení:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Průvodce odstraňováním potíží a [Řešení potíží s dokumentem.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="e588e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="e588e-122">[Zjistěte, jak zaregistrovat zařízení s Windows v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="e588e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
