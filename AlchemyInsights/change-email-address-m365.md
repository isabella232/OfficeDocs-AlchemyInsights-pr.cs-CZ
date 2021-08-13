---
title: Změna e-mailové adresy skupiny Microsoftu 365 nebo Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995615"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Změna e-mailové adresy skupiny Microsoftu 365 nebo Microsoft Teams

E-mailovou adresu skupiny Microsoftu 365 nebo Microsoft Teams můžete změnit v [Centru pro správu Microsoftu 365](https://admin.microsoft.com/). Stačí vybrat skupinu a pak vybrat @upravit e-mailovou adresu.

Ke změně primární SMTP adresy skupiny Microsoftu 365 nebo Teams můžete použít i následující příkaz EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Příklad:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
