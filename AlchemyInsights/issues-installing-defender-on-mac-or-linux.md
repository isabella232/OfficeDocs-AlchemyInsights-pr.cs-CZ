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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539673"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémy s instalací Microsoft Defenderu na Mac nebo Linux

**Mac**

- Před instalací aplikace Microsoft Defender ATP pro Mac se ujistěte, že jsou splněny požadavky na systém. Další informace najdete v [článku Jak nainstalovat Microsoft Defender ATP pro Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Zkontrolujte informace v souboru: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Před instalací systému pro Linux se ujistěte, že jsou Microsoft Defender ATP požadavky na systém. Další informace najdete v [článku Jak nainstalovat MDATP pro Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Informace o tom, MDATP služba spuštěná, najdete v [tématu Instalace se nezdařila.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Pokud chcete vyřešit a vyřešit problémy, pokud služba není spuštěná, podívejte se na postup řešení potíží, pokud služba [mdatp není spuštěná.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Postup kontroly konfigurace klienta, který ověřuje stav produktu, a spuštění detekčního testu v textovém souboru EICAR najdete v tématu [Konfigurace klienta](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Poznámka:** Seznam podporovaných souborových systémů pro aktivitu při přístupu najdete v Microsoft Defender ATP [pro Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).