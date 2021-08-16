---
title: Zapnutí auditování poštovní schránky
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058031"
---
# <a name="turn-on-mailbox-auditing"></a>Zapnutí auditování poštovní schránky

Pokud chcete zapnout auditování poštovních schránek pro jednoho uživatele nebo celou organizaci, spusťte následující rutiny ze vzdáleného PowerShellu:

- **Jeden uživatel:** Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organizace:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Další informace najdete v tématu [Správa auditování poštovní schránky](https://go.microsoft.com/fwlink/?linkid=2103668).