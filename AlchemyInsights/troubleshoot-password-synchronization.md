---
title: Poradce při potížích se synchronizací hesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105741"
---
# <a name="troubleshoot-password-synchronization"></a>Poradce při potížích se synchronizací hesel

Pokud chcete vyřešit problémy se synchronizací hesel, začněte tím, že Připojení AAD a zjistěte, proč se hesla nesynchronují. Začněte tak, že přejděte na [Spravovat přímou synchronizaci](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otevřete novou relaci Windows PowerShell na serveru Azure AD Připojení a vyberte **možnost Spustit jako** správce.

2. Spusťte Set-ExecutionPolicy RemoteSigned nebo Set-ExecutionPolicy Unrestricted.

3. Spusťte průvodce Azure AD Připojení Azure AD.

4. Přejděte na stránku Další úkoly a > **Poradce při**  >  **potížích s dalším.**

5. Výběrem **možnosti Spustit** otevřete nabídku řešení potíží s PowerShellem.

6. Vyberte **Poradce při potížích se synchronizací hesel.**

    Problém je obvykle v tom, že se heslo pro konkrétní uživatelský účet nesynchronuje.

    **Poznámky** Synchronizace hesel se nezdaří, pokud byla poslední úspěšná synchronizace hesel před nějakou dobou.

Další informace o řešení potíží se synchronizací hesel najdete v tématu Řešení potíží se synchronizací hodnot hash hesel se synchronizací [Připojení Azure AD.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)