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
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818461"
---
# <a name="change-strong-password-requirement"></a>Změna požadavků na silné heslo

Microsoft ve výchozím nastavení vyžaduje silná hesla.

Pomocí PowerShellu můžete zakázat silná hesla pro konkrétní uživatele pomocí těchto příkazů:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Pokud chcete zakázat silná hesla pro všechny uživatele, použijte:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Další informace o zásadách hesel](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Jak se připojit k Microsoftu 365 pomocí PowerShellu](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Další informace o příkazech PowerShellu MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
