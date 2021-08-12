---
title: Odesílatel nepřijímá e-maily odeslané Microsoft 365 skupině.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958290"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Odesílatel nepřijímá e-maily odeslané Microsoft 365 skupině.

Odesílatel e-mailové zprávy do skupiny Microsoft 365 ve výchozím nastavení neobdrží kopii zprávy ve složce Doručená pošta, a to ani v případě, že je odesílatel členem skupiny.

Pomocí tohoto příkazu EXO PowerShell můžete odesílateli povolit, aby obdržel kopii každého e-mailu, který pošle Microsoft 365 skupině:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Povolení nastavení pro všechny poštovní schránky najednou:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Poznámka:** Změny tohoto nastavení se projeví až za hodinu.