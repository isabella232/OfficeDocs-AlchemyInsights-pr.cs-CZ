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
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Poradce při potížích s registrací zařízení s Windows v Microsoft Intune

Prohlédněte si níže uvedené zdroje a problém vyřešte.
  
Některé běžné chybové zprávy a postupy řešení:
  
 **Software nelze nainstalovat, 0x80cf4017:** Vypršela platnost vašeho certifikátu účtu. Balíček softwaru pro klientský software znovu stáhněte v konzoli pro správu Intune. Další informace najdete v této dokumentaci.
  
 **Kód chyby 0x801c0003:** K chybě může dojít v následujících situacích:
  
-  Uživatel má více popsaných zařízení, než je limit zařízení. Pokud chcete [Odebrat zařízení](https://docs.microsoft.com/intune/devices-wipe) nebo [změnit limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), Projděte si tyto dokumenty.

-  "Uživatelé se mohou připojovat do služby Azure AD" jsou nastaveny na "none". Nastavte ho na všichni nebo vyberte uživatele. Další informace najdete v [této dokumentaci](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Zařízení je už zaregistrované jiným uživatelem. V takovém případě odeberte zařízení z konzoly Azure Intune nebo ručně zrušte registraci zařízení a potom to zkuste znovu.

-  Zařízení je Windows 10 Home. Do Azure Active Directory se můžou připojit jenom Windows 10 pro, vzdělávací a Enterprise SKU.

Další zdroje informací pro řešení vašeho problému:
  
-  Na [portálu Poradce při potížích s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby zápisu. Další podrobnosti najdete v [tomto dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .

-  V těchto dokumentech se podívejte na seznam běžných chyb, které zabraňují zápisu a řešení každého z nich: [Poradce při potížích](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [odstraňování potíží s dokumentem](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Naučte se zapisovat zařízení s Windows v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
