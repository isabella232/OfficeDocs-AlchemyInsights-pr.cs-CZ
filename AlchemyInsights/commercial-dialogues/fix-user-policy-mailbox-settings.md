---
title: Oprava nastavení zásad uživatele/poštovní schránky
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744842"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="2f1ec-102">Oprava nastavení zásad uživatele/poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="2f1ec-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="2f1ec-103">Tato zpráva se týká nastavení nevyžádané pošty v poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="2f1ec-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="2f1ec-104">Nastavení si můžete zkontrolovat takto:</span><span class="sxs-lookup"><span data-stu-id="2f1ec-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="2f1ec-105">Spusťte Prostředí Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="2f1ec-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="2f1ec-106">Další informace najdete v tématu [Otevření prostředí Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="2f1ec-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="2f1ec-107">Spusťte tento příkaz (pomocí e-mailové adresy uživatele):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="2f1ec-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="2f1ec-108">Zkontrolujte, jestli je e-mailová adresa odesílatele součástí **TrustedSendersAndDomains** nebo **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="2f1ec-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="2f1ec-109">Pokud je e-mailová adresa v jednom ze seznamů, možná ji budete muset odebrat.</span><span class="sxs-lookup"><span data-stu-id="2f1ec-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="2f1ec-110">Další informace najdete v tématu [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="2f1ec-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
