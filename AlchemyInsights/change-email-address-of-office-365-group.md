---
title: Změna e-mailové adresy skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580650"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Změna e-mailové adresy skupiny Microsoft 365

E-mailovou adresu skupiny Microsoft 365 můžete změnit pomocí Centra pro správu. Stačí vybrat skupinu a vybrat @edit e-mailovou adresu.

Pomocí následujícího příkazu EXO PowerShell můžete také změnit primární adresu SMTP skupiny Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Příklad:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
