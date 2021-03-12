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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744657"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Řešení problémů s instalací MDATP na Macu

Pokud ruční instalace selže, **zobrazí se na** stránce Souhrn v průvodci instalací tato chyba:

"Při instalaci došlo k chybě. Instalační program zjistil chybu, která způsoboval selhání instalace. Požádejte o pomoc výrobce softwaru."

U nasazení MDM se na stránce zobrazuje i obecná chyba instalace.

I když se koncovým uživatelům nezobrazují přesné chyby, udržme soubor protokolu s průběhem instalace v **/Library/Logs/Microsoft/mdatp/install.log**. Každá instalační relace se připojí k tomuto souboru protokolu. Pokud chcete vysílovat jenom poslední relaci instalace, použijte `sed` .

Další informace najdete v tématu Řešení potíží s [instalací pro microsoft defender atp pro Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
