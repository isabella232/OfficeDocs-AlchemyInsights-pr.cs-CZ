---
title: Poradce při potížích s registrací zařízení s Windows v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665825"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="c74ca-102">Poradce při potížích s registrací zařízení s Windows v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c74ca-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="c74ca-103">Problém nyní vyřešte v následujících zdrojích.</span><span class="sxs-lookup"><span data-stu-id="c74ca-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c74ca-104">Některé běžné chybové zprávy a kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="c74ca-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="c74ca-105">**Software nelze nainstalovat, 0x80cf4017:** Platnost certifikátu účtu vypršela.</span><span class="sxs-lookup"><span data-stu-id="c74ca-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="c74ca-106">Znovu si stáhněte softwarový balíček klienta počítače v Konzole pro správu Intune.</span><span class="sxs-lookup"><span data-stu-id="c74ca-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="c74ca-107">Další informace naleznete v této dokumentaci.</span><span class="sxs-lookup"><span data-stu-id="c74ca-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="c74ca-108">**Kód chyby 0x801c0003:** K chybě může dojít v následujících scénářích:</span><span class="sxs-lookup"><span data-stu-id="c74ca-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="c74ca-109">Uživatel má více zařízení zaregistrovaných, než je limit zařízení.</span><span class="sxs-lookup"><span data-stu-id="c74ca-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c74ca-110">Chcete-li [odebrat zařízení](https://docs.microsoft.com/intune/devices-wipe) nebo [změnit limit zařízení ,](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)zkontrolujte tyto dokumenty .</span><span class="sxs-lookup"><span data-stu-id="c74ca-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="c74ca-111">"Uživatelé mohou připojit zařízení k Azure AD" je nastavena na "žádný."</span><span class="sxs-lookup"><span data-stu-id="c74ca-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="c74ca-112">Nastavte ji na všechny nebo vyberte uživatele.</span><span class="sxs-lookup"><span data-stu-id="c74ca-112">Set it to all or select users.</span></span> <span data-ttu-id="c74ca-113">Další informace naleznete [v této dokumentaci.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)</span><span class="sxs-lookup"><span data-stu-id="c74ca-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="c74ca-114">Zařízení je již zaregistrováno jiným uživatelem.</span><span class="sxs-lookup"><span data-stu-id="c74ca-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="c74ca-115">Pokud tomu tak je, odeberte zařízení z konzoly Azure Intune nebo ručně zrušit registraci zařízení před další pokusy.</span><span class="sxs-lookup"><span data-stu-id="c74ca-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="c74ca-116">Zařízení je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="c74ca-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="c74ca-117">Azure Active Directory se můžou připojit jenom skutek pro Windows 10 Pro, Education a Enterprise.</span><span class="sxs-lookup"><span data-stu-id="c74ca-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="c74ca-118">Další zdroje informací, které vám pomohou problém vyřešit:</span><span class="sxs-lookup"><span data-stu-id="c74ca-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="c74ca-119">Pomocí [portálu pro řešení potíží s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a řešit běžné chyby registrace.</span><span class="sxs-lookup"><span data-stu-id="c74ca-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c74ca-120">Další podrobnosti naleznete v [tomto dokumentu.](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="c74ca-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="c74ca-121">V těchto dokumentech naleznete seznam běžných chyb, které brání zápisu a řešení jednotlivých položek: [Průvodce odstraňováním potíží](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Odstraňování potíží s dokumenty](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c74ca-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="c74ca-122">[Přečtěte si, jak zaregistrovat zařízení s Windows v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="c74ca-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
