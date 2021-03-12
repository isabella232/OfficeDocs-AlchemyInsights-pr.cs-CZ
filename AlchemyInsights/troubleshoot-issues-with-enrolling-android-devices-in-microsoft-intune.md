---
title: Poradce při potížích s zaregistrovat zařízení s Androidem v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708991"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Poradce při potížích s zaregistrovat zařízení s Androidem v Microsoft Intune

Pokud chcete problém vyřešit hned, zkontrolujte níže uvedené zdroje informací.
  
Některé běžné problémy a kroky řešení:
  
 **Chyba Šifrované zařízení na portálu společnosti:** Novější verze Androidu, konkrétně od verze 7.0, vyžadují přístupové heslo při spuštění, aby bylo vaše zařízení plně zašifrované. Běžnými řešeními je povolit připnutí při spuštění nebo plně zašifrovat zařízení. Další [informace najdete v](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) tomto dokumentu.
  
 **Zařízení se nepodaří služby Intune** zkontrolovat nebo se v konzole pro správu Intune zobrazí jako není v pořádku: Některá zařízení Samsung 4.4 a 5.5 nemusí služby zkontrolovat. Existují 3 možná řešení tohoto problému:
  
1. Ručně otevřete aplikaci Portál společnosti Intune, která automaticky spustí synchronizaci zařízení.

2. Aktualizujte zařízení na Android 6.0 nebo vyšší.

3. Zakažte Samsung Smart Manageru správu portálu společnosti Intune. Další [podrobnosti o těchto](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) problémech a řešeních najdete v tomto dokumentu.

 **Chyba typu Neplatná licence** nebo **Uživatelské jméno:** Uživatel musí mít přiřazenou licenci Intune nebo EMS. Tyto dokumenty si projdete a přiřadíte licenci prostřednictvím: Centra pro správu Office nebo portálu Azure Portal.
  
Další zdroje informací, které vám pomůžou problém vyřešit:
  
1. Pomocí [portálu Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby registrace. Další [podrobnosti najdete v](https://docs.microsoft.com/intune/help-desk-operators) tomto dokumentu.

2. V [tomto dokumentu se](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) můžete se seznamem běžných chyb, které brání zápisu a řešení každého z nich.

3. [Zjistěte, jak zaregistrovat zařízení s Androidem v Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
