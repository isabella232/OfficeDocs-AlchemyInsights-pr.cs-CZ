---
title: Vlastník nemůže vytvořit podsložku pomocí Outlooku.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665711"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlastník nemůže vytvořit podsložku pomocí Outlooku.

**U vlastníků veřejných složek se při vytváření podsložek používá Outlook. Problém bude brzy opraven.**

Dále použijte jedno z následujících řešení:

1. Vytvoření podsložky pomocí Outlooku pro MAC jenom Outlook pro desktopová okna (všechny verze)
2. Vytvoření podsložky pomocí Správce EXO Shell nebo EAC
3. Změnit DefaultPublicFolderMailbox/EffectivePublicFolderMailbox u uživatele na jinou poštovní schránku, než je poštovní schránka pro složku, která způsobuje chybu  
    - *Set-Mailbox user1 DefaultPublicFolderMailbox PubMBX3*
4. Počkat na hodinu, restartovat klienta Outlooku