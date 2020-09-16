---
title: Změna e-mailové adresy skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733680"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Změna e-mailové adresy skupiny Microsoft 365

E-mailovou adresu skupiny Microsoft 365 můžete změnit pomocí centra pro správu. Vyberte skupinu a vyberte @edit e-mailová adresa.

Primární adresu SMTP skupiny Microsoft 365 můžete změnit taky pomocí příkazu EXO PowerShellu:

Set-Unified <Group Name> -PrimarySMTPAddress <new SMTP Address>

Pøíklad

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
