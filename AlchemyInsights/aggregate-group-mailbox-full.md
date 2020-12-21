---
title: AggregateGroupMailbox byla přijata úplná nedoručená zpráva pro e-mail odeslaný do skupiny Microsoft 365.
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721782"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox byla přijata úplná nedoručená zpráva pro e-mail odeslaný do skupiny Microsoft 365.

Pomocí následujícího příkazu EXO Shell vytvoříte pravidlo přenosu Exchange pro tiché vyřazení e-mailů odeslaných do agregované poštovní schránky skupiny:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Nahraďte adresu SMTP v **-SentTo** pomocí adresy SMTP agregované poštovní schránky skupiny ve vašem tenantovi. Adresu SMTP agregované poštovní schránky skupiny můžete získat z doručené pošty.



