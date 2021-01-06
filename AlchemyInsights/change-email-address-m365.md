---
title: Změna e-mailové adresy skupiny Microsoftu 365 nebo Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756550"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Změna e-mailové adresy skupiny Microsoftu 365 nebo Microsoft Teams

E-mailovou adresu skupiny Microsoftu 365 nebo Microsoft Teams můžete změnit v [Centru pro správu Microsoftu 365](https://admin.microsoft.com/). Stačí vybrat skupinu a pak vybrat @upravit e-mailovou adresu.

Ke změně primární SMTP adresy skupiny Microsoftu 365 nebo Teams můžete použít i následující příkaz EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Příklad:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
