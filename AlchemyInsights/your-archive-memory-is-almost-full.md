---
title: Vaše archivní poštovní schránka je skoro plná
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974212"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="08f63-102">Vaše archivní poštovní schránka je skoro plná</span><span class="sxs-lookup"><span data-stu-id="08f63-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="08f63-103">Pokud uživatel obdrží upozornění; **Vaše archivní poštovní schránka je skoro plná** nebo potřebujete zvětšit velikost archivované poštovní schránky:</span><span class="sxs-lookup"><span data-stu-id="08f63-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="08f63-104">Pokud je uživateli přiřazený online plán 1, upgradujte na licenci **Exchange Online Plan 2** , abyste zvýšili velikost z 50 GB na 100GB.</span><span class="sxs-lookup"><span data-stu-id="08f63-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="08f63-105">Pokud je uživatel už přiřazený: **Exchange Online (plán 2** ) nebo Exchange Online (plán 1) s doplňkem Exchange Online pro archivaci, použijte k povolení automatického rozbalování archivování následující postup:</span><span class="sxs-lookup"><span data-stu-id="08f63-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="08f63-106">[Připojení k PowerShellu služby Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="08f63-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="08f63-107">Pro uživatele spusťte následující unifiedgroup:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="08f63-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="08f63-108">Potvrďte povolení pro uživatele spuštěním následujícího unifiedgroup:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="08f63-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="08f63-109">Další informace najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="08f63-109">For more information see:</span></span>

- [<span data-ttu-id="08f63-110"> Povolit neomezené archivace – Nápověda pro správce – dodržování předpisů Microsoft 365 | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="08f63-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="08f63-111">Limity pro Exchange Online – popisy služeb | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="08f63-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="08f63-112">Upgrade na jiný firemní plán | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="08f63-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

