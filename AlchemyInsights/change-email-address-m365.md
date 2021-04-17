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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819073"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Změna e-mailové adresy skupiny Microsoftu 365 nebo Microsoft Teams

E-mailovou adresu skupiny Microsoftu 365 nebo Microsoft Teams můžete změnit v [Centru pro správu Microsoftu 365](https://admin.microsoft.com/). Stačí vybrat skupinu a pak vybrat @upravit e-mailovou adresu.

Ke změně primární SMTP adresy skupiny Microsoftu 365 nebo Teams můžete použít i následující příkaz EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Příklad:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
