---
title: Změna e-mailové adresy Microsoft 365 skupiny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930722"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Změna e-mailové adresy Microsoft 365 skupiny

E-mailovou adresu skupiny Microsoft 365 můžete změnit pomocí Centra pro správu. Stačí vybrat skupinu a pak vybrat @upravit e-mailovou adresu.

Pomocí příkazu EXO PowerShell můžete taky změnit primární adresu SMTP Microsoft 365 skupiny:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Příklad:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
