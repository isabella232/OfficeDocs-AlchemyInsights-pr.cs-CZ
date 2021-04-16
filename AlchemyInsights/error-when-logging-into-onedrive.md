---
title: 0x8004de40 při spuštění OneDrivu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813645"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 při spuštění OneDrivu

Pokud se při přihlašování **0x8004de40** OneDrivu zobrazí chybová zpráva, restartujte počítač při připojení k vaší pracovní nebo školní doméně. Pokud se po restartování zobrazí tato chyba, zkuste to, když jste připojení k vaší pracovní nebo školní doméně:

1. Klikněte na Start a  do vyhledávacího pole zadejte **cmd** nebo příkazový řádek, klikněte pravým tlačítkem myši na aplikaci příkazového řádku a vyberte **Spustit jako správce**. Pokud se zobrazí výzva k zadání hesla správce nebo k potvrzení, zadejte heslo nebo klikněte na **Povolit.**  

2. V okně Příkazového řádku zadejte **dsregcmd /leave**  a počkejte, až se příkaz dokončí. Potom zadejte **dsregcmd /join** a počkejte, až se příkaz dokončí.
3. Restartujte počítač.
