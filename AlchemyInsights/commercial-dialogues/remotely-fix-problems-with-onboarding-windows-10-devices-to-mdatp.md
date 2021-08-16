---
title: Vzdáleně opravte problémy s připojením Windows 10 zařízení do programu Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034027"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Vzdáleně opravte problémy s připojením Windows 10 zařízení do programu Microsoft Defender Advanced Threat Protection

Pokud máte přístup ke vzdálenému počítači, postupujte takto:

1. Stáhněte si diagnostický nástroj [Client Connectivity Analyzer.](https://go.microsoft.com/fwlink/?linkid=2143466)
2. Extrahujte a spusťte MDATPAnalyzer.cmd.
3. Vyhledejte diagnostický protokol ve složce MDATPClientAnalyzerResult, což je stejná složka, ve které byl nástroj Analyzer stažen.
4. Pokud chcete najít problémy s připojením nebo nastavením internetového proxy serveru, zkontrolujte soubor protokolu MDATPClientAnalyzer.txt.

Další informace najdete v tématu Problémy s počítači s [připojením.](https://go.microsoft.com/fwlink/?linkid=2143634)
