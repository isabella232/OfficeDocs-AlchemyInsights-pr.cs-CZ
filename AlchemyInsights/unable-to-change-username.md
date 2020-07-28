---
title: Nelze změnit uživatelské jméno.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439098"
---
# <a name="unable-to-change-username"></a>Nelze změnit uživatelské jméno.

V některých případech změny hlavního názvu uživatele (UserPrincipalName) nejsou šířeny do cloudu. Na portálu Office 365 se mohou zobrazit chyby ověření nebo nemůžete změnit uživatelské jméno nebo e-mailovou adresu. Chcete-li tento problém vyřešit, nastavte ručně UserPrincipalName pomocí tohoto příkazu prostředí PowerShell.

**Příklad: Přejmenování uživatele**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Tento příkaz davidc@contoso.com přejmenuje na davidchew@contoso.com.

Další informace naleznete v [tématu Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).