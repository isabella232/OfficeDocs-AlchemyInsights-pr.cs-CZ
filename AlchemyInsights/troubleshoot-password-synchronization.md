---
title: Poradce při potížích se synchronizací hesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387870"
---
# <a name="troubleshoot-password-synchronization"></a>Poradce při potížích se synchronizací hesel

Chcete-li vyřešit problémy se synchronizací hesel, začněte pomocí této úlohy řešení potíží služby AAD Connect a zjistěte, proč se hesla nesynchronizují. Začněte tak, že přejdete na [Spravovat přímou synchronizaci](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otevřete novou relaci prostředí Windows PowerShell na serveru Azure AD Connect a vyberte možnost **Spustit jako správce.**

2. Spustit set-executionPolicy RemoteSigned nebo Set-ExecutionPolicy Unrestricted.

3. Spusťte Průvodce azure ad připojení.

4. Přejděte na stránku Další úkoly > **Poradce při potížích s**  >  **dalšími**úkoly .

5. Výběrem **možnosti Spustit** otevřete nabídku řešení potíží s PowerShellem.

6. Vyberte **Možnost Poradce při potížích se synchronizací hesel**.

    Problém je obvykle, že heslo není synchronizován pro konkrétní uživatelský účet.

    **Poznámky** Synchronizace hesel se nezdaří, pokud poslední úspěšná synchronizace hesel byla před nějakým časem.

Další informace o řešení potíží se synchronizací hesel najdete [v tématu Poradce při potížích se synchronizací hash hesel se synchronizací Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).