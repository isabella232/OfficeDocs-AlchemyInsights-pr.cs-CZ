---
title: AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315903"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group

Pomocí následujícího příkazu PROSTŘEDÍ EXO můžete vytvořit pravidlo přenosu Exchange, aby se e-maily odeslané do agregované poštovní schránky skupiny bezobslužně přemisťují:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Poznámka:** Nahraďte adresu SMTP v **části -SentTo** adresou SMTP agregované poštovní schránky skupiny ve vašem tenantovi. Adresu SMTP agregované poštovní schránky skupiny můžete získat z přijatého oznámení o nedoručení.



