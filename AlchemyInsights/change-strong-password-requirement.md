---
title: Změnit požadavek silného hesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804416"
---
# <a name="change-strong-password-requirement"></a>Změnit požadavek silného hesla

Microsoft vyžaduje ve výchozím nastavení silné heslo.

Pomocí PowerShellu můžete zakázat silná hesla pro určité uživatele pomocí těchto příkazů:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Pokud chcete zakázat silná hesla pro všechny uživatele, použijte:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Další informace o zásadách hesel](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Jak se připojit k Microsoft 365 pomocí PowerShellu](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Další informace o příkazech MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
