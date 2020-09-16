---
title: Obnovení odstraněných položek pomocí rutiny
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741296"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="d0580-102">Obnovení odstraněných položek pomocí rutiny</span><span class="sxs-lookup"><span data-stu-id="d0580-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="d0580-103">K zobrazení odstraněných položek v poštovních schránkách použijte rutinu [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) .</span><span class="sxs-lookup"><span data-stu-id="d0580-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="d0580-104">Po vyhledání odstraněných položek pomocí rutiny [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) je obnovíte.</span><span class="sxs-lookup"><span data-stu-id="d0580-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="d0580-105">Podívejte se na úplné podrobnosti v [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d0580-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="d0580-106">Abyste mohli spustit tuto rutinu, musíte mít přiřazenou roli exportovat import poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="d0580-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="d0580-107">Další informace najdete v článku [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) .</span><span class="sxs-lookup"><span data-stu-id="d0580-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
