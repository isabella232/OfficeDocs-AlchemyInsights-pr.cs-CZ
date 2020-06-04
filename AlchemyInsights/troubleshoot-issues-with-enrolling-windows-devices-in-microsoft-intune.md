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
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Poradce při potížích s registrací zařízení s Windows v Microsoft Intune

Problém nyní vyřešte v následujících zdrojích.
  
Některé běžné chybové zprávy a kroky řešení:
  
 **Software nelze nainstalovat, 0x80cf4017:** Platnost certifikátu účtu vypršela. Znovu si stáhněte softwarový balíček klienta počítače v Konzole pro správu Intune. Další informace naleznete v této dokumentaci.
  
 **Kód chyby 0x801c0003:** K chybě může dojít v následujících scénářích:
  
-  Uživatel má více zařízení zaregistrovaných, než je limit zařízení. Chcete-li [odebrat zařízení](https://docs.microsoft.com/intune/devices-wipe) nebo [změnit limit zařízení ,](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)zkontrolujte tyto dokumenty .

-  "Uživatelé mohou připojit zařízení k Azure AD" je nastavena na "žádný." Nastavte ji na všechny nebo vyberte uživatele. Další informace naleznete [v této dokumentaci.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)

-  Zařízení je již zaregistrováno jiným uživatelem. Pokud tomu tak je, odeberte zařízení z konzoly Azure Intune nebo ručně zrušit registraci zařízení před další pokusy.

-  Zařízení je Windows 10 Home. Azure Active Directory se můžou připojit jenom skutek pro Windows 10 Pro, Education a Enterprise.

Další zdroje informací, které vám pomohou problém vyřešit:
  
-  Pomocí [portálu pro řešení potíží s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a řešit běžné chyby registrace. Další podrobnosti naleznete v [tomto dokumentu.](https://docs.microsoft.com/intune/help-desk-operators)

-  V těchto dokumentech naleznete seznam běžných chyb, které brání zápisu a řešení jednotlivých položek: [Průvodce odstraňováním potíží](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Odstraňování potíží s dokumenty](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Přečtěte si, jak zaregistrovat zařízení s Windows v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
