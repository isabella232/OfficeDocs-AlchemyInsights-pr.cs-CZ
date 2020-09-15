---
title: Poradce při potížích s registrací zařízení s Windows v Microsoft Intune
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658871"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="72edb-102">Poradce při potížích s registrací zařízení s Windows v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="72edb-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="72edb-103">Prohlédněte si níže uvedené zdroje a problém vyřešte.</span><span class="sxs-lookup"><span data-stu-id="72edb-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="72edb-104">Některé běžné chybové zprávy a postupy řešení:</span><span class="sxs-lookup"><span data-stu-id="72edb-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="72edb-105">**Software nelze nainstalovat, 0x80cf4017:** Vypršela platnost vašeho certifikátu účtu.</span><span class="sxs-lookup"><span data-stu-id="72edb-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="72edb-106">Balíček softwaru pro klientský software znovu stáhněte v konzoli pro správu Intune.</span><span class="sxs-lookup"><span data-stu-id="72edb-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="72edb-107">Další informace najdete v této dokumentaci.</span><span class="sxs-lookup"><span data-stu-id="72edb-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="72edb-108">**Kód chyby 0x801c0003:** K chybě může dojít v následujících situacích:</span><span class="sxs-lookup"><span data-stu-id="72edb-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="72edb-109">Uživatel má více popsaných zařízení, než je limit zařízení.</span><span class="sxs-lookup"><span data-stu-id="72edb-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="72edb-110">Pokud chcete [Odebrat zařízení](https://docs.microsoft.com/intune/devices-wipe) nebo [změnit limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), Projděte si tyto dokumenty.</span><span class="sxs-lookup"><span data-stu-id="72edb-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="72edb-111">"Uživatelé se mohou připojovat do služby Azure AD" jsou nastaveny na "none".</span><span class="sxs-lookup"><span data-stu-id="72edb-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="72edb-112">Nastavte ho na všichni nebo vyberte uživatele.</span><span class="sxs-lookup"><span data-stu-id="72edb-112">Set it to all or select users.</span></span> <span data-ttu-id="72edb-113">Další informace najdete v [této dokumentaci](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="72edb-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="72edb-114">Zařízení je už zaregistrované jiným uživatelem.</span><span class="sxs-lookup"><span data-stu-id="72edb-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="72edb-115">V takovém případě odeberte zařízení z konzoly Azure Intune nebo ručně zrušte registraci zařízení a potom to zkuste znovu.</span><span class="sxs-lookup"><span data-stu-id="72edb-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="72edb-116">Zařízení je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="72edb-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="72edb-117">Do Azure Active Directory se můžou připojit jenom Windows 10 pro, vzdělávací a Enterprise SKU.</span><span class="sxs-lookup"><span data-stu-id="72edb-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="72edb-118">Další zdroje informací pro řešení vašeho problému:</span><span class="sxs-lookup"><span data-stu-id="72edb-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="72edb-119">Na [portálu Poradce při potížích s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby zápisu.</span><span class="sxs-lookup"><span data-stu-id="72edb-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="72edb-120">Další podrobnosti najdete v [tomto dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="72edb-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="72edb-121">V těchto dokumentech se podívejte na seznam běžných chyb, které zabraňují zápisu a řešení každého z nich: [Poradce při potížích](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [odstraňování potíží s dokumentem](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="72edb-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="72edb-122">[Naučte se zapisovat zařízení s Windows v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="72edb-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
