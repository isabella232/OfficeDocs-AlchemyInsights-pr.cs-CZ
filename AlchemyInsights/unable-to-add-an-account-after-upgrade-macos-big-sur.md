---
title: Po upgradu na macOS 11.6 Big Sur se nedaří přidat účet.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506251"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Po upgradu na macOS 11.6 Big Sur se nedaří přidat účet.

Po upgradu na macOS 11.6 se váš OneDrive pro pracovní nebo školní účet nebo váš osobní účet OneDrive nemusí v seznamu účtů zobrazit a možná se nebudete moct přihlásit k druhému účtu z aplikace.

Pro tento problém byla vyvinuta oprava. Nejdřív určete, jestli používáte samostatnou verzi nebo verzi app storu OneDrive:

- V řádku nabídek vyberte OneDrive cloud a > **nápovědy & Nastavení**  >  **Předvolby**  >  **o aplikaci**. Pokud číslo verze neobsahuje **(samostatný),** máte verzi produktu z App Storu.

Pokud používáte samostatnou verzi aplikace OneDrive, restartujte počítač a OneDrive automatické aktualizace buildu, ve kterém je tento problém vyřešen. Pokud chcete build nainstalovat ručně, stáhněte si tento soubor.zip , rozbalte soubor [a](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)zkopírujte aplikaci OneDrive do složky Aplikace (nahrazením stávající OneDrive aplikace).

Pokud používáte verzi App Storu, zvažte instalaci samostatné verze OneDrive. Tato verze funguje stejně jako verze App Storu, ale umožňuje Microsoftu nabízet uživatelům aktualizace rychleji a připojit je k verzi, která obsahuje opravu tohoto problému.

1. Stáhněte si samostatnou [verzi OneDrive, která obsahuje opravu](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. Rozbalte soubor a zkopírujte aplikaci OneDrive do složky Aplikace (nahrazením stávající OneDrive aplikace).

Pokud potřebujete použít verzi App Storu, počkejte, až App Store uvolní verzi aplikace, která obsahuje opravu. Microsoft bohužel nemůže sdělit odhadované datum vydání pevné verze z App Storu.


