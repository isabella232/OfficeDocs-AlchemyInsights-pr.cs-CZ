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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="84ec4-102">Odesílatel neobdrží e-maily odeslané do skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="84ec4-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="84ec4-103">Ve výchozím nastavení neobdrží odesílatel e-mailové zprávy skupině Microsoft 365 kopii zprávy v doručené poště ani v případě, že je odesílatel členem skupiny.</span><span class="sxs-lookup"><span data-stu-id="84ec4-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="84ec4-104">Pomocí tohoto EXO příkazu PowerShellu umožníte odesílateli obdržet kopii každého e-mailu, který odešle skupině Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="84ec4-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="84ec4-105">Povolení nastavení pro všechny poštovní schránky najednou:</span><span class="sxs-lookup"><span data-stu-id="84ec4-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="84ec4-106">**Poznámka:** Změny tohoto nastavení se projeví až za hodinu.</span><span class="sxs-lookup"><span data-stu-id="84ec4-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>