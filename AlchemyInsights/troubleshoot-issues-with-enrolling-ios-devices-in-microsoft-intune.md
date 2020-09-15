---
title: Poradce při potížích s registrací zařízení iOS v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669241"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Poradce při potížích s registrací zařízení iOS v Microsoft Intune

Prohlédněte si níže uvedené zdroje a problém vyřešte. 
  
Některé běžné chybové zprávy a postupy řešení:
  
- **Zakončení zařízení** Uživatel má více popsaných zařízení, než je limit zařízení. Pokud chcete [Odebrat zařízení](https://docs.microsoft.com/intune/devices-wipe) nebo [změnit limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), Projděte si tyto dokumenty.
    
- **Tato služba není podporovaná. Žádné zásady zápisu:** službu APNs (Apple Push Notification Service) je třeba nakonfigurovat nebo obnovit. V [tomto dokumentu](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) najdete pokyny, jak to udělat. 
    
- **Typ uživatelské licence není platný nebo nejde rozpoznat uživatelské jméno:** Uživateli musí být přiřazena licence Intune nebo EMS. V těchto dokumentech si můžete přiřadit licenci pomocí [centra pro správu Office](https://docs.microsoft.com/intune/licenses-assign) nebo [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Další zdroje informací pro řešení vašeho problému:
  
1. Na [portálu Poradce při potížích s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby zápisu. Další podrobnosti najdete v [tomto dokumentu](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. V těchto dokumentech se podívejte na seznam běžných chyb, které zabraňují zápisu a řešení každého z nich: [Poradce při potížích](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [odstraňování potíží s dokumentem](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Naučte se zapisovat zařízení s iOS v Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

