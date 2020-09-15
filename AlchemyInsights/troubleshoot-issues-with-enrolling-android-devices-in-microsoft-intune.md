---
title: Poradce při potížích s registrací zařízení s Androidem v Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689947"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Poradce při potížích s registrací zařízení s Androidem v Microsoft Intune

Prohlédněte si níže uvedené zdroje a problém vyřešte.
  
Některé běžné problémy a řešení:
  
 **Chyba nešifrovaného zařízení na portálu společnosti:** Novější verze Androidu, zejména od verze 7.0, vyžadují spouštěcí heslo, abyste měli jistotu, že vaše zařízení je plně šifrované. Běžná řešení: Povolte spouštěcí PIN nebo plně Zašifrujte zařízení. V [tomto dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) najdete další informace.
  
 Zařízení se nepovedlo **vrátit se změnami a zobrazit jako "v nesprávném stavu" v konzoli správce Intune:** Některá zařízení Samsung 4,4 a 5,5 nemusí tuto službu vrátit. Existuje 3 možná řešení tohoto problému:
  
1. Ručně otevřete aplikaci Portál společnosti Intune, která automaticky zahájí synchronizaci zařízení.

2. Aktualizujte zařízení na Android 6,0 nebo novější.

3. Zakažte čipovou kartu Samsung pro správu portálu společnosti Intune. V [tomto dokumentu](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) najdete další podrobnosti o těchto problémech a řešeních.

 **Typ uživatelské licence není platný** nebo **došlo k neznámé chybě uživatelského jména:** uživateli musí být přiřazena licence Intune nebo EMS. V těchto dokumentech si můžete přiřadit licenci pomocí centra pro správu Office nebo Azure Portal.
  
Další zdroje informací pro řešení vašeho problému:
  
1. Na [portálu Poradce při potížích s Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) můžete diagnostikovat a vyřešit běžné chyby zápisu. Další podrobnosti najdete v [tomto dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .

2. V [tomto dokumentu](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) se zobrazí seznam běžných chyb, které se zabrání zápisu a řešení každého z nich.

3. [Naučte se zapisovat zařízení s Androidem v Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
