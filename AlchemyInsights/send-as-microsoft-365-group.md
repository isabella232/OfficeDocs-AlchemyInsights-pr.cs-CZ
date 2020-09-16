---
title: Odeslat jako skupinu Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740144"
---
# <a name="send-as-microsoft-365-group"></a>Odeslat jako skupinu Microsoft 365

Pokud chcete, aby konkrétní uživatelé odesílali zprávy jako skupinu Microsoft 365, můžete přiřadit oprávnění Odeslat jako:  

1. Připojení k PowerShellu služby Exchange Online  

2. Spusťte tento příkaz:  

    Add-RecipientPermission `<GroupName>` -oprávněný uživatel `<MailboxName>` AccessRights SendAs

Další informace najdete v tématu [Povolení odesílání nebo posílání členům ve skupině](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).