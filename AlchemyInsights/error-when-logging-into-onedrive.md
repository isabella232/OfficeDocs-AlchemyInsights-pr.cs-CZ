---
title: 0x8004de40 při spuštění OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946572"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 při spuštění OneDrive

Pokud se při přihlašování **0x8004de40** k OneDrive, restartujte počítač při připojení k vaší pracovní nebo školní doméně. Pokud se po restartování zobrazí tato chyba, zkuste to, když jste připojení k vaší pracovní nebo školní doméně:

1. Klikněte na Start a  do vyhledávacího pole zadejte **cmd** nebo příkazový řádek, klikněte pravým tlačítkem myši na aplikaci příkazového řádku a vyberte **Spustit jako správce**. Pokud se zobrazí výzva k zadání hesla správce nebo k potvrzení, zadejte heslo nebo klikněte na **Povolit.**  

2. V okně Příkazového řádku zadejte **dsregcmd /leave**  a počkejte, až se příkaz dokončí. Potom zadejte **dsregcmd /join** a počkejte, až se příkaz dokončí.
3. Restartujte počítač.
