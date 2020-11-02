---
title: Chyba 0x8004de40 při spouštění OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823015"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>Chyba 0x8004de40 při spouštění OneDrivu

Pokud se při přihlašování k OneDrivu zobrazí chybová zpráva **0x8004de40** , restartujte počítač, když jste připojení k vaší pracovní nebo školní doméně. Pokud se tato chyba zobrazí po restartování počítače, vyzkoušejte to, co se připojuje k vaší pracovní nebo školní doméně:

1. Klikněte na Start a do vyhledávacího pole zadejte **cmd** nebo **Command Prompt**  , klikněte pravým tlačítkem na aplikaci příkazového řádku a vyberte  **Spustit jako správce** . Pokud se zobrazí výzva k zadání hesla správce nebo potvrzení, zadejte heslo nebo klikněte na **Povolit** .  

2. V okně příkazového řádku zadejte **dsregcmd/Leave**  a počkejte, až se příkaz dokončí. Potom zadejte **dsregcmd/JOIN** a počkejte, až se příkaz dokončí.
3. Restartujte počítač.
