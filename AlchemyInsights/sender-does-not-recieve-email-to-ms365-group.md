---
title: Odesílatel neobdrží e-maily odeslané do skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871668"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Odesílatel neobdrží e-maily odeslané do skupiny Microsoft 365

Ve výchozím nastavení neobdrží odesílatel e-mailové zprávy skupině Microsoft 365 kopii zprávy v doručené poště ani v případě, že je odesílatel členem skupiny.

Pomocí tohoto EXO příkazu PowerShellu umožníte odesílateli obdržet kopii každého e-mailu, který odešle skupině Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Povolení nastavení pro všechny poštovní schránky najednou:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Poznámka:** Změny tohoto nastavení se projeví až za hodinu.