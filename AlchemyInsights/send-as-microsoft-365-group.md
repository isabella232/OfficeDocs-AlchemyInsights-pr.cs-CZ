---
title: Odeslat jako skupinu Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871670"
---
# <a name="send-as-microsoft-365-group"></a>Odeslat jako skupinu Microsoft 365

Pokud chcete, aby konkrétní uživatelé odesílali zprávy jako skupinu Microsoft 365, můžete přiřadit oprávnění Odeslat jako:  

1. Připojení k PowerShellu služby Exchange Online  

2. Spusťte tento příkaz:  

    Add-RecipientPermission `<GroupName>` -oprávněný uživatel `<MailboxName>` AccessRights SendAs

Další informace najdete v tématu [Povolení odesílání nebo posílání členům ve skupině](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).