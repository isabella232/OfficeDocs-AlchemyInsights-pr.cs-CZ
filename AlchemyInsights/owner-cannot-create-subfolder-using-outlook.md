---
title: Vlastník nemůže vytvořit podsadu pomocí Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063117"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlastník nemůže vytvořit podsadu pomocí Outlook

**Dochází k probíhajícímu problému s vytvářením podsložek pomocí Outlook. Problém bude brzy opravený.**

Mezitím použijte jedno z následujících alternativních řešení:

1. Použití Outlook pro MAC k vytvoření podsložky, protože problém se týká jenom Outlook pro desktopová okna (všechny verze)
2. Vytvoření podsložky správcem pomocí prostředí EXO Shell nebo EAC
3. Změna DefaultPublicFolderMailbox/EffectivePublicFolderMailbox u uživatele na jinou poštovní schránku než poštovní schránku obsahu pro složku způsobující problém  
    - *Set-Mailbox User1 DefaultPublikaceMailbox PubMBX3*
4. Počkejte hodinu, restartujte klienta Outlooku.