---
title: Send As Microsoft 365 group
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
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086121"
---
# <a name="send-as-microsoft-365-group"></a>Send As Microsoft 365 group

Oprávnění Odeslat jako můžete přiřadit konkrétním uživatelům, aby mohli posílat zprávy jako Microsoft 365 skupiny:  

1. Připojení k Exchange Online PowerShellu.  

2. Spusťte následující příkaz:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Další informace najdete v článku [Povolení členům](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)odesílat jako skupinu nebo je posílat jménem skupiny .