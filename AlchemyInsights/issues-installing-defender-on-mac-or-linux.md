---
title: Problémy s instalací Microsoft Defenderu na Mac nebo Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013237"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémy s instalací Microsoft Defenderu na Mac nebo Linux

**Mac**

- Před instalací programu Microsoft Defender ATP pro Mac se ujistěte, že jsou splněny požadavky na systém. Další informace najdete v tématu Instalace programu [Microsoft Defender ATP pro Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Zkontrolujte informace v souboru: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Před instalací programu Microsoft Defender ATP pro Linux se ujistěte, že jsou splněny požadavky na systém. Další informace najdete v [článku Jak nainstalovat MDATP pro Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Informace o tom, jestli je služba MDATP spuštěná, najdete v [článku Instalace se nezdařila.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Pokud chcete vyřešit a vyřešit problémy, pokud služba není spuštěná, podívejte se na postup řešení potíží, pokud služba [mdatp není spuštěná.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Postup kontroly konfigurace klienta, který ověřuje stav produktu, a spuštění detekčního testu v textovém souboru EICAR najdete v tématu [Konfigurace klienta](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Poznámka:** Seznam podporovaných souborových systémů pro aktivitu při přístupu najdete v tématu [Microsoft Defender ATP pro Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).