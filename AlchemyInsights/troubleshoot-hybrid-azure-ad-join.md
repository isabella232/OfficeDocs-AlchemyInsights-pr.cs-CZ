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
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939264"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Řešení potíží s hybridním připojením k Azure AD

Důrazně doporučujeme Zajistit, aby zařízení měla přístup ke koncovým bodům registrace zařízení pod systémovým účtem pomocí skriptu Připojení k registraci [testovacího zařízení](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Pokud registrace zařízení nastavujete poprvé, přečtěte si článek I[ntroduction to device management](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) in Azure Active Directory to learn how to get devices under the control of Azure AD .)
1. Pokud přímo zaregistrujete zařízení do Azure AD a zaregistrujete je do Intune, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) ujistěte se, že jste nakonfigurovali [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a měli jste na prvním místě licencování.
1. Ujistěte se, že máte oprávnění provádět operace v Azure AD a místní službě AD. Nastavení pro registrace zařízení může spravovat jenom globální správce v Azure AD. Pokud navíc nastavujete automatické registrace v místní službě Active Directory, musíte být správcem služby Active Directory a služby AD FS (pokud je to možné).

Další podrobnosti o řešení potenciálních problémů [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) s hybridním připojením najdete v tématu Řešení potíží s hybridním připojením k hybridnímu připojení pro nastavení hybridních zařízení připojených k Azure AD a správa zařízení pomocí portálu Azure Ad, najdete v článku Nastavení hybridních zařízení připojených k [Azure AD (místních doménových)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) a Správa zařízení pomocí [portálu Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Pokud chcete vyřešit běžné problémy s hybridním připojením Azure Active Directory (AD), podívejte se na časté otázky k [připojení k hybridní službě Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)
