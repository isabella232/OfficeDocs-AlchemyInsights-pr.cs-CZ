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
# <a name="unable-to-change-username"></a><span data-ttu-id="393e6-102">Nelze změnit uživatelské jméno.</span><span class="sxs-lookup"><span data-stu-id="393e6-102">Unable to change UserName</span></span>

<span data-ttu-id="393e6-103">V některých případech změny hlavního názvu uživatele (UserPrincipalName) nejsou šířeny do cloudu.</span><span class="sxs-lookup"><span data-stu-id="393e6-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="393e6-104">Na portálu Office 365 se mohou zobrazit chyby ověření nebo nemůžete změnit uživatelské jméno nebo e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="393e6-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="393e6-105">Chcete-li tento problém vyřešit, nastavte ručně UserPrincipalName pomocí tohoto příkazu prostředí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="393e6-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="393e6-106">**Příklad: Přejmenování uživatele**</span><span class="sxs-lookup"><span data-stu-id="393e6-106">**Example: Rename a user**</span></span>

<span data-ttu-id="393e6-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="393e6-107">PowerShellCopy</span></span>

<span data-ttu-id="393e6-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="393e6-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="393e6-109">Tento příkaz davidc@contoso.com přejmenuje na davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="393e6-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="393e6-110">Další informace naleznete v [tématu Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="393e6-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>