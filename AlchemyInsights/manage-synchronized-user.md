---
title: Správa synchronizovaných uživatelů
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114764"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nelze nastavit primární e-mailovou adresu, změnit atributy uživatele nebo odebrat nebo odstranit synchronizované uživatele.

Pokud je pro vaše prostředí povolená synchronizace adresářů, nelze některé atributy uživatele nebo objektu změnit pomocí Centrum pro správu Microsoftu 365.

Pokud chcete synchronizované uživatele a všechny jejich atributy plně spravovat, použijte místní uživatele služby Active Directory a konzolu pro správu skupin (adsiedit.msc).  

Můžete také změnit jednotlivé uživatele nebo atributy synchronizovaných uživatelů pomocí powershellu, jak je vidět v těchto běžných příkladech:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
