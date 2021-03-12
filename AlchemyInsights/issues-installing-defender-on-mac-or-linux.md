---
title: Problémy s instalací programu Microsoft Defender na Mac nebo Linux
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713388"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problémy s instalací programu Microsoft Defender na Mac nebo Linux

**Mac**

- Před instalací atp pro Mac v programu Microsoft Defender se ujistěte, že jsou splněné požadavky na systém. Další informace najdete v článku o instalaci programu [Microsoft Defender ATP pro Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Zkontrolujte informace v souboru: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Před instalací programu Microsoft Defender ATP pro Linux ověřte, že jsou splněné požadavky na systém. Další informace najdete v článku o instalaci programu [Microsoft Defender ATP pro Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Pokud chcete ověřit, jestli je služba MDATP spuštěná, podívejte se, [jestli se instalace nezdařila.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Pokud chcete vyřešit a vyřešit problémy, pokud služba není spuštěná, podívejte se na postup řešení, pokud služba [mdatp není spuštěná.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Postup pro kontrolu konfigurace klienta, který ověří stav produktu, a spuštění testovacího zjišťování u textového souboru EICAR, najdete v [části Konfigurace klienta.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Poznámka** Seznam podporovaných souborových systémů pro aktivitu při přístupu najdete v programu [Microsoft Defender ATP pro Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)