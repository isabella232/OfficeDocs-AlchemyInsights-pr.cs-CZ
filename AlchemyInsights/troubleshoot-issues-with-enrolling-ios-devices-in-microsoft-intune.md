---
title: Poradce při potížích s registraci zařízení s iOSem v Microsoft Intune
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708955"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Poradce při potížích s registraci zařízení s iOSem v Microsoft Intune

Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací. 
  
Některé běžné chybové zprávy a kroky řešení:
  
- **Dosáhli jste limitu zařízení** Uživatel má zaregistrované víc zařízení, než je limit počtu zařízení. V těchto dokumentech můžete [odebrat zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) změnit limit [zařízení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Tato služba není podporovaná. Žádné zásady registrace: Služba** nabízených oznámení Apple (APNS) se musí nakonfigurovat nebo prodloužit. Pokyny [k tomu najdete](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) v tomto dokumentu. 
    
- **Neplatný typ uživatelské licence nebo uživatelské jméno není rozpoznáno:** Uživatel musí mít přiřazenou licenci k Intune nebo EMS. Tyto dokumenty si projdete a přiřadíte licenci prostřednictvím: [Centra pro správu Office](https://docs.microsoft.com/intune/licenses-assign) nebo portálu Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Další zdroje informací, které vám pomůžou problém vyřešit:
  
1. Pomocí [portálu Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby registrace. Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu. 
    
2. V těchto dokumentech najdete seznam běžných chyb, které zabraňují jejich zápisu a [řešení:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Průvodce odstraňováním potíží a [Řešení potíží s dokumentem.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Zjistěte, jak zaregistrovat zařízení s iOSem v Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

