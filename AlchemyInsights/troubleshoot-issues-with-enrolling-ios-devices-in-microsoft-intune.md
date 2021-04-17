---
title: Řešení problémů s registracemi zařízení s iOSem v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823456"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Řešení problémů s registracemi zařízení s iOSem v Microsoft Intune

Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací. 
  
Některé běžné chybové zprávy a kroky řešení:
  
- **Bylo dosaženo krytu zařízení** Uživatel má zaregistrovaná víc zařízení, než je limit zařízení. Zkontrolujte tyto dokumenty a [odeberte zařízení nebo](https://docs.microsoft.com/intune/devices-wipe) [změňte limit zařízení](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Tato služba není podporovaná. Žádné zásady registrace:** Služba APNS (Apple Push Notification Service) musí být nakonfigurovaná nebo obnovená. Pokyny [k tomu najdete](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) v tomto dokumentu. 
    
- **Typ uživatelské licence: Neplatné nebo Uživatelské jméno není rozpoznáno:** Uživateli je potřeba přiřadit licenci Intune nebo EMS. Projděte si tyto dokumenty a přiřaďte licenci prostřednictvím: [Centra pro](https://docs.microsoft.com/intune/licenses-assign) správu Office nebo portálu [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Další zdroje informací, které vám pomůžou problém vyřešit:
  
1. K [diagnostice a](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) řešení běžných chyb registrace použijte Portál řešení potíží s Intune. Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu. 
    
2. V těchto dokumentech najdete seznam běžných chyb, které brání zápisu a řešení jednotlivých dokumentů: [Průvodce](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) odstraňováním potíží a [Poradce při potížích s dokumentem](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Zjistěte, jak zaregistrovat zařízení s iOSem v Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

