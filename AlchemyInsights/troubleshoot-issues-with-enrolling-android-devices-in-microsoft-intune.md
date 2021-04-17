---
title: Řešení problémů s registracemi zařízení s Androidem v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830935"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Řešení problémů s registracemi zařízení s Androidem v Microsoft Intune

Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.
  
Některé běžné problémy a kroky řešení:
  
 **Chyba zařízení není šifrovaná na portálu společnosti:** Novější verze Androidu, zejména od verze 7.0, vyžadují spouštěcí heslo, aby bylo zařízení plně zašifrované. Běžnými řešeními je povolit připnutí při spuštění nebo plně zašifrovat zařízení. Další [informace najdete v tomto](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dokumentu.
  
 **Zařízení se nedaří se službou Intune** zkontrolovat nebo se v konzole pro správu Intune nezobrazovat jako "Není v pořádku": Některá zařízení Samsung 4.4 a 5.5 nemusí službu zkontrolovat. Existují 3 možná řešení tohoto problému:
  
1. Ručně otevřete aplikaci Portál společnosti Intune, která automaticky zahájí synchronizaci zařízení.

2. Aktualizujte zařízení na Android 6.0 nebo novější.

3. Zakažte Samsung Smart Manageru ve správě portálu společnosti Intune. Další [podrobnosti o těchto](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) problémech a řešeních najdete v tomto dokumentu.

 **User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Projděte si tyto dokumenty a přiřaďte licenci prostřednictvím: Centra pro správu Office nebo portálu Azure Portal.
  
Další zdroje informací, které vám pomůžou problém vyřešit:
  
1. K [diagnostice a](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) řešení běžných chyb registrace použijte Portál řešení potíží s Intune. Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.

2. V [tomto dokumentu se](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) můžete se seznamem běžných chyb, které brání zápisu a jejich řešení.

3. [Zjistěte, jak zaregistrovat zařízení s Androidem v Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
