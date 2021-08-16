---
title: Dávka migrace veřejné složky se stavem CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068157"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Dávka migrace veřejné složky se stavem CompletedWithErrors

K dokončení dávky použijte následující postup a přeskočte velké nebo špatné položky: 
1. Schválení vynechaných položek v dávce migrace:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. K schválení vynechaných položek u žádostí o migraci, které jsou synchronizované, ale nejsou dokončené, použijte následující příkaz:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Dávka migrace a žádosti by měly pokračovat a dokončit během několika minut.

