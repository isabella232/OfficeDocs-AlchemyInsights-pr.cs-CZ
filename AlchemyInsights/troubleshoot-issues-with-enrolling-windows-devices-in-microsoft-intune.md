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
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Poradce při potížích s registraci zařízení s Windows v Microsoft Intune

Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.
  
Některé běžné chybové zprávy a kroky řešení:
  
 **Software nelze nainstalovat, 0x80cf4017:** Platnost certifikátu účtu vypršela. V konzole pro správu Intune znovu stáhněte softwarový balíček Klienta počítače. Další informace najdete v této dokumentaci.
  
 **Kód chyby 0x801c0003:** K chybě může dojít v následujících situacích:
  
-  Uživatel má zaregistrované víc zařízení, než je limit počtu zařízení. V těchto dokumentech můžete [odebrat zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) změnit limit [zařízení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  Možnost "Uživatelé mohou připojit zařízení k Azure AD" je nastavena na hodnotu "žádný". Nastavte ji na všechny uživatele nebo vyberte uživatele. Další [informace najdete v](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) této dokumentaci.

-  Zařízení už zaregistroval jiný uživatel. V takovém případě odeberte zařízení z konzoly Azure Intune nebo ho před pokusem znovu ručně derollujte.

-  Zařízení je Windows 10 Home. K Azure Active Directory se může připojit jenom skladové soubory Windows 10 Pro, Education a Enterprise.

Další zdroje informací, které vám pomůžou problém vyřešit:
  
-  Pomocí [portálu Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby registrace. Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.

-  V těchto dokumentech najdete seznam běžných chyb, které zabraňují jejich zápisu a [řešení:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Průvodce odstraňováním potíží a [Řešení potíží s dokumentem.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Zjistěte, jak zaregistrovat zařízení s Windows v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
