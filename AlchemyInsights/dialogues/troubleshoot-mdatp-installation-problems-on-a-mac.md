---
title: Řešení problémů s instalací MDATP na Macu
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693350"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Řešení problémů s instalací MDATP na Macu

Pokud se ruční instalace **nezdaří,** zobrazí se na stránce Souhrn v Průvodci instalací tato chybová zpráva:

"Při instalaci došlo k chybě. Instalační program narazil na chybu, která způsoboval selhání instalace. Požádejte o pomoc výrobce softwaru."

U nasazení MDM se na stránce zobrazuje také obecná chyba instalace.

Ačkoli koncovým uživatelům nezobrazujíme přesné chyby, uchováme soubor protokolu s průběhem instalace v **umístění /Library/Logs/Microsoft/mdatp/install.log.** Každá instalační relace se připojí k tomuto souboru protokolu. Pokud chcete výstupovat jenom poslední relaci instalace, použijte `sed` .

Další informace najdete v článku Řešení potíží s [instalací nástroje Microsoft Defender ATP pro Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
