---
title: Řešení problémů s registracem Windows zařízení v Microsoft Intune
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
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981034"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Řešení problémů s registracem Windows zařízení v Microsoft Intune

Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.
  
Některé běžné chybové zprávy a kroky řešení:
  
 **Software nelze nainstalovat, 0x80cf4017:** Platnost certifikátu vašeho účtu vypršela. Znovu stáhněte softwarový balíček Klienta počítače v konzole pro správu Intune. Další informace najdete v této dokumentaci.
  
 **Kód chyby 0x801c0003:** K chybě může dojít v následujících situacích:
  
-  Uživatel má zaregistrovaná víc zařízení, než je limit zařízení. Zkontrolujte tyto dokumenty a [odeberte zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) [změňte limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Uživatelé se smí připojit k Azure AD" je nastavené na "žádné". Nastavte ho na všechny nebo vyberte uživatele. Další [informace najdete v](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) této dokumentaci.

-  Zařízení už zaregistroval jiný uživatel. V takovém případě odeberte zařízení z konzoly Azure Intune nebo zařízení před znova ručně derollujte.

-  Zařízení je Windows 10 Home. K Windows 10 Pro se mohou připojit jenom Enterprise, Education a Azure Active Directory.

Další zdroje informací, které vám pomůžou problém vyřešit:
  
-  K [diagnostice a](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) řešení běžných chyb registrace použijte Portál řešení potíží s Intune. Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.

-  V těchto dokumentech najdete seznam běžných chyb, které brání zápisu a řešení jednotlivých dokumentů: [Průvodce](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) odstraňováním potíží a [Poradce při potížích s dokumentem](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Zjistěte, jak zaregistrovat Windows zařízení v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
