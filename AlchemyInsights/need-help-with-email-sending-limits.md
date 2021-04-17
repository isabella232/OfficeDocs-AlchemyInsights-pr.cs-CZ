---
title: Potřebujete pomoct s limity odesílání e-mailů?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836272"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="9e23d-102">Potřebujete pomoct s limity odesílání e-mailů?</span><span class="sxs-lookup"><span data-stu-id="9e23d-102">Need help with email sending limits?</span></span>

<span data-ttu-id="9e23d-103">Dole jsou **limity odesílání podle návrhu** vynucované ve službě.</span><span class="sxs-lookup"><span data-stu-id="9e23d-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="9e23d-104">Další informace o těchto limitech najdete [tady.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="9e23d-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="9e23d-105">Aby nedoručovaly nevyžádané hromadné zprávy, používáme limity sazeb pro příjemce pro všechny odchozí a **interní zprávy**.</span><span class="sxs-lookup"><span data-stu-id="9e23d-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="9e23d-106">V rámci všech skladové velikosti je tento limit **10 000 příjemců denně**.</span><span class="sxs-lookup"><span data-stu-id="9e23d-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="9e23d-107">Zákazníci, kteří potřebují posílat legitimní hromadně komerční e-maily (například bulletiny zákazníků), by měli používat poskytovatele třetích stran, kteří se na tyto služby specializují.</span><span class="sxs-lookup"><span data-stu-id="9e23d-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="9e23d-108">**Poznámka:** Po dosažení limitu počtu příjemců se zprávy z poštovní schránky neposílat, dokud se počet příjemců, kteří byli odeslaných zpráv za posledních 24 hodin, pod tento limit klesne.</span><span class="sxs-lookup"><span data-stu-id="9e23d-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="9e23d-109">Uživatel nebude moct odesílat zprávy až do tohoto okamžiku.</span><span class="sxs-lookup"><span data-stu-id="9e23d-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="9e23d-110">Limit rychlosti zpráv **30 zpráv za minutu** se použije ve všech skladových skladových velikosti.</span><span class="sxs-lookup"><span data-stu-id="9e23d-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="9e23d-111">Určuje, kolik zpráv může uživatel během určitého období odeslat ze svého účtu Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9e23d-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="9e23d-112">Maximální **počet příjemců povolených** v polích Komu, Kopie a Skrytá pro jednu e-mailovou zprávu ve všech skladových položek je **1 000 příjemců**.</span><span class="sxs-lookup"><span data-stu-id="9e23d-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="9e23d-113">Pokud chcete tento limit přizpůsobit, přejděte [sem](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="9e23d-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
