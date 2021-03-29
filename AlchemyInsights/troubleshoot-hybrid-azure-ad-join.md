---
title: Řešení potíží s hybridním připojením k Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401900"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="d1057-102">Řešení potíží s hybridním připojením k Azure AD</span><span class="sxs-lookup"><span data-stu-id="d1057-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="d1057-103">Důrazně doporučujeme Zajistit, aby zařízení měla přístup ke koncovým bodům registrace zařízení pod systémovým účtem pomocí skriptu Připojení k registraci [testovacího zařízení](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="d1057-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="d1057-104">Pokud registrace zařízení nastavujete poprvé, přečtěte si článek Úvod ke správě zařízení ve[službě Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) a zjistěte, jak získat zařízení pod kontrolou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d1057-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="d1057-105">Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) ujistěte se, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a měli jste na prvním místě licencování.</span><span class="sxs-lookup"><span data-stu-id="d1057-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="d1057-106">Ujistěte se, že máte oprávnění provádět operace v Azure AD a místní službě AD.</span><span class="sxs-lookup"><span data-stu-id="d1057-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="d1057-107">Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d1057-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="d1057-108">Pokud navíc nastavujete automatické registrace v místní službě Active Directory, musíte být správcem služby Active Directory a služby AD FS (pokud je to možné).</span><span class="sxs-lookup"><span data-stu-id="d1057-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="d1057-109">Další podrobnosti o řešení potenciálních problémů [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) s hybridním připojením najdete v tématu Řešení potíží s hybridním připojením k hybridnímu připojení pro nastavení hybridních zařízení připojených k Azure AD a správa zařízení pomocí portálu Azure Ad, najdete v článku Nastavení hybridních zařízení připojených k [Azure AD (místních doménových)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) a Správa zařízení pomocí [portálu Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d1057-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="d1057-110">Pokud chcete vyřešit běžné problémy s hybridním připojením ke službě Azure Active Directory (AD), podívejte se na [časté otázky k připojení k hybridní službě Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)</span><span class="sxs-lookup"><span data-stu-id="d1057-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
