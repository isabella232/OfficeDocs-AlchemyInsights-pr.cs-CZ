---
title: Potřebujete pomoct s limity odesílání e-mailů?
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
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702356"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="01e47-102">Potřebujete pomoct s limity odesílání e-mailů?</span><span class="sxs-lookup"><span data-stu-id="01e47-102">Need help with email sending limits?</span></span>

<span data-ttu-id="01e47-103">Níže je uvedený **limit odesílání v rámci návrhu vydaný** službou.</span><span class="sxs-lookup"><span data-stu-id="01e47-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="01e47-104">Další informace o těchto limitech [najdete tady](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="01e47-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="01e47-105">Aby se zabránilo doručování nevyžádaných hromadných zpráv, platíme **pro všechny odchozí a interní zprávy**.</span><span class="sxs-lookup"><span data-stu-id="01e47-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="01e47-106">U všech skladových položek je tento limit **10 000 příjemců za den**.</span><span class="sxs-lookup"><span data-stu-id="01e47-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="01e47-107">Zákazníci, kteří potřebují odesílat legitimní komerční e-maily (například zákaznické zpravodaje), by měli používat poskytovatele třetích stran, kteří v těchto službách specializují.</span><span class="sxs-lookup"><span data-stu-id="01e47-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="01e47-108">**Poznámka**: po dosažení limitu přenosové rychlosti není možné z poštovní schránky odesílat zprávy, dokud neklesne do počtu příjemců, kteří poslali zprávy během posledních 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="01e47-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="01e47-109">Uživatel nebude moct odesílat zprávy do tohoto místa.</span><span class="sxs-lookup"><span data-stu-id="01e47-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="01e47-110">Limit počtu zpráv: **30 zpráv za minutu** se používá ve všech skladových jednotkách.</span><span class="sxs-lookup"><span data-stu-id="01e47-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="01e47-111">Tento způsob určuje, kolik zpráv může uživatel posílat z účtu Exchange Online v zadaném období.</span><span class="sxs-lookup"><span data-stu-id="01e47-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="01e47-112">**Maximální počet příjemců povolený v polích Komu, kopie a skrytá** pro jednu e-mailovou zprávu ve všech skladových jednotkách je **1000**.</span><span class="sxs-lookup"><span data-stu-id="01e47-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="01e47-113">Pokud chcete tento limit přizpůsobit, přejděte [sem](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="01e47-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
