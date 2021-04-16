---
title: Povolení auditování poštovní schránky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814185"
---
# <a name="enable-mailbox-auditing"></a>Povolení auditování poštovní schránky

Pokud chcete povolit auditování poštovních schránek pro jednoho uživatele nebo pro celou organizaci, musí být ze vzdáleného prostředí Power Shell spuštěny následující rutiny:
  
 **Jeden uživatel**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **Organizace**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Víc se uč](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

