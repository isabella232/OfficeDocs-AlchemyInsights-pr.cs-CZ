---
title: Vlastník nemůže vytvořit podsadu pomocí Outlooku.
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836128"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlastník nemůže vytvořit podsadu pomocí Outlooku.

**Při vytváření podsložek pomocí Outlooku dochází k probíhajícímu problému s vlastníky veřejných složek. Problém bude brzy opravený.**

Mezitím použijte jedno z následujících alternativních řešení:

1. Vytvoření podsložky v Outlooku pro MAC se týká jenom Outlooku pro desktopová okna (všechny verze).
2. Vytvoření podsložky správcem pomocí prostředí EXO Shell nebo EAC
3. Změna DefaultPublicFolderMailbox/EffectivePublicFolderMailbox u uživatele na jinou poštovní schránku než poštovní schránku obsahu pro složku způsobující problém  
    - *Set-Mailbox User1 DefaultPublikaceMailbox PubMBX3*
4. Počkejte hodinu, restartujte klienta Outlooku.