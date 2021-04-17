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
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823960"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nelze nastavit primární e-mailovou adresu, změnit atributy uživatele nebo odebrat nebo odstranit synchronizované uživatele.

Pokud je pro vaše prostředí povolená synchronizace adresářů, není možné změnit některé atributy uživatelů nebo objektů pomocí Centra pro správu Microsoftu 365.

Pokud chcete synchronizované uživatele a všechny jejich atributy plně spravovat, použijte místní uživatele služby Active Directory a konzolu pro správu skupin (adsiedit.msc).  

Můžete také změnit jednotlivé uživatele nebo atributy synchronizovaných uživatelů pomocí powershellu, jak je vidět v těchto běžných příkladech:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
