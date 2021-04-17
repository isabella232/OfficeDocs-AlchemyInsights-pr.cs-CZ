---
title: Obnovení odstraněných položek rutinou
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835804"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="61cc3-102">Obnovení odstraněných položek rutinou</span><span class="sxs-lookup"><span data-stu-id="61cc3-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="61cc3-103">K zobrazení odstraněných položek v poštovních schránkách použijte rutinu [Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="61cc3-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="61cc3-104">Po vyhledání odstraněných položek je můžete obnovit pomocí rutiny [Restore-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="61cc3-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="61cc3-105">Podrobnosti najdete v [tématu Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="61cc3-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="61cc3-106">Abyste mohli tuto rutinu spustit, musíte mít přiřazenou roli Export importu poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="61cc3-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="61cc3-107">Další informace najdete v tématu [Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="61cc3-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
