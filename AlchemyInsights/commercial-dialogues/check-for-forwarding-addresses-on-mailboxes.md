---
title: Kontrola přeposílání adres v poštovních schránkách
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403304"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="68b83-102">Kontrola přeposílání adres v poštovních schránkách</span><span class="sxs-lookup"><span data-stu-id="68b83-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="68b83-103">Někdy hackeři přeposílání e-mailových zpráv uživatelů sami sobě, takže nejdřív zkontrolujeme přeposílání adres a pravidel pro poštovní schránku.</span><span class="sxs-lookup"><span data-stu-id="68b83-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="68b83-104">Pak zkontrolujeme protokoly auditování.</span><span class="sxs-lookup"><span data-stu-id="68b83-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="68b83-105">Tady je postup, jak zkontrolovat přeposílání adres:</span><span class="sxs-lookup"><span data-stu-id="68b83-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="68b83-106">Vyberte **Uživatelé**  >  **aktivní uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="68b83-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="68b83-107">Vyberte uživatele, jehož účet byl ohrožen.</span><span class="sxs-lookup"><span data-stu-id="68b83-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="68b83-108">V plovoucím seznamu, který se zobrazí, rozbalte **Nastavení pošty** a potom klikněte **na Upravit** pro přeposílání **e-mailů.**</span><span class="sxs-lookup"><span data-stu-id="68b83-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="68b83-109">Odeberte všechny adresy pro přeposílání, které nepoznáváte.</span><span class="sxs-lookup"><span data-stu-id="68b83-109">Remove any forwarding addresses you don't recognize.</span></span>