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
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898601"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémy s instalací Microsoft Defenderu na Mac nebo Linux

**Mac**

- Před instalací programu Microsoft Defender ATP pro Mac se ujistěte, že jsou splněny požadavky na systém. Další informace najdete v tématu Instalace programu [Microsoft Defender ATP pro Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Zkontrolujte informace v souboru: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Před instalací programu Microsoft Defender ATP pro Linux se ujistěte, že jsou splněny požadavky na systém. Další informace najdete v [článku Jak nainstalovat MDATP pro Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Informace o tom, jestli je služba MDATP spuštěná, najdete v [článku Instalace se nezdařila.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Pokud chcete vyřešit a vyřešit problémy, pokud služba není spuštěná, podívejte se na postup řešení potíží, pokud služba [mdatp není spuštěná.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Postup kontroly konfigurace klienta, který ověřuje stav produktu, a spuštění detekčního testu v textovém souboru EICAR najdete v tématu [Konfigurace klienta](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Poznámka:** Seznam podporovaných souborových systémů pro aktivitu při přístupu najdete v tématu [Microsoft Defender ATP pro Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).