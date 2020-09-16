---
title: Pro dávku migrace veřejné složky se stavem CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744106"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pro dávku migrace veřejné složky se stavem CompletedWithErrors

Dávku dokončíte provedením následujících kroků, které vynechají velké/špatné položky: 
1. Schválení vynechaných položek v dávce migrace:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Pomocí následujícího příkazu schválíte přeskočené položky u žádostí o migraci, které jsou synchronizované, ale ne dokončené:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Dávka a žádosti o migraci by měly být v průběhu několika minut obnoveny.

