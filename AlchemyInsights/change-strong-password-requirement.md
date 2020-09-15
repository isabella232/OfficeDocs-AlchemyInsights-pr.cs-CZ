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
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681865"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="4ffe4-102">Změnit požadavek silného hesla</span><span class="sxs-lookup"><span data-stu-id="4ffe4-102">Change strong password requirement</span></span>

<span data-ttu-id="4ffe4-103">Microsoft vyžaduje ve výchozím nastavení silné heslo.</span><span class="sxs-lookup"><span data-stu-id="4ffe4-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="4ffe4-104">Pomocí PowerShellu můžete zakázat silná hesla pro určité uživatele pomocí tohoto příkazu:</span><span class="sxs-lookup"><span data-stu-id="4ffe4-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="4ffe4-105">*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="4ffe4-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="4ffe4-106">Další informace o zásadách hesel</span><span class="sxs-lookup"><span data-stu-id="4ffe4-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="4ffe4-107">Jak se připojit k Microsoft 365 pomocí PowerShellu</span><span class="sxs-lookup"><span data-stu-id="4ffe4-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="4ffe4-108">Další informace o příkazech MsolUser</span><span class="sxs-lookup"><span data-stu-id="4ffe4-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
