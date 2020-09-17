---
title: Správa synchronizovaných uživatelů
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777670"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nelze nastavit primární e-mailovou adresu, změnit atributy uživatele nebo odebrat či odstranit synchronizovaného uživatele.

Pokud je synchronizace adresářů pro vaše prostředí povolená, některé atributy uživatelů nebo objektů se nedají změnit pomocí centra pro správu Microsoft 365.

Chcete-li spravovat synchronizované uživatele a všechny jejich atributy, použijte konzolu pro správu Uživatelé a skupiny služby Active Directory (adsiedit. msc).  

Můžete taky změnit jednotlivé uživatele nebo atributy pro synchronizované uživatele pomocí PowerShellu, jako je to vidět v těchto běžných příkladech: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
