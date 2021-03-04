---
title: Kontrola přeposílání adres u poštovních schránek
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427131"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="3c4b9-102">Kontrola přeposílání adres u poštovních schránek</span><span class="sxs-lookup"><span data-stu-id="3c4b9-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="3c4b9-103">Někdy hackeři přeposílání e-mailových zpráv uživatelů sami sobě, takže nejdřív zkontrolujeme přeposílání adres a pravidel pro poštovní schránku.</span><span class="sxs-lookup"><span data-stu-id="3c4b9-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="3c4b9-104">Potom zkontrolujeme protokoly auditování.</span><span class="sxs-lookup"><span data-stu-id="3c4b9-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="3c4b9-105">Tady je postup, jak zkontrolovat přeposílání adres:</span><span class="sxs-lookup"><span data-stu-id="3c4b9-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="3c4b9-106">Vyberte **Aktivní**  >  **uživatelé.**</span><span class="sxs-lookup"><span data-stu-id="3c4b9-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="3c4b9-107">Vyberte uživatele, u kterého byl ohrožen účet.</span><span class="sxs-lookup"><span data-stu-id="3c4b9-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="3c4b9-108">V oznámení, které se zobrazí, rozbalte **nastavení** pošty a potom klikněte na **Upravit** pro **přeposílání e-mailů.**</span><span class="sxs-lookup"><span data-stu-id="3c4b9-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="3c4b9-109">Odeberte všechny adresy pro přeposílání, které nepoznáte.</span><span class="sxs-lookup"><span data-stu-id="3c4b9-109">Remove any forwarding addresses you don't recognize.</span></span>