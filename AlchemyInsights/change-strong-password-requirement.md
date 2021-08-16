---
title: Změna požadavků na silné heslo
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
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070677"
---
# <a name="change-strong-password-requirement"></a>Změna požadavků na silné heslo

Microsoft ve výchozím nastavení vyžaduje silná hesla.

Pomocí PowerShellu můžete zakázat silná hesla pro konkrétní uživatele pomocí těchto příkazů:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Pokud chcete zakázat silná hesla pro všechny uživatele, použijte:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Další informace o zásadách hesel](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Jak se připojit k Microsoft 365 pomocí PowerShellu](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Další informace o příkazech PowerShellu MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
