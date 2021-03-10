---
title: Oprava pravidel pro adresu odesílatele nebo seznam domén
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
ms.openlocfilehash: a57016ce0b5e8ed741889a50e3858c68578c6713
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693357"
---
# <a name="fix-sender-addressdomain-list-rules"></a><span data-ttu-id="6a75c-102">Oprava pravidel pro adresu odesílatele nebo seznam domén</span><span class="sxs-lookup"><span data-stu-id="6a75c-102">Fix Sender Address/Domain list rules</span></span>

<span data-ttu-id="6a75c-103">Tato zpráva se týká zásady ochrany proti nevyžádané poště ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="6a75c-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="6a75c-104">Odesílatel zprávy byl nalezen v seznamu Povolit nebo Blokovat.</span><span class="sxs-lookup"><span data-stu-id="6a75c-104">The sender of the message was found in an Allow or Block list.</span></span> <span data-ttu-id="6a75c-105">Chcete-li tyto zásady zkontrolovat, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="6a75c-105">To review the policy, do the following:</span></span>

1. <span data-ttu-id="6a75c-106">Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143)potom přejděte na Zásady řízení rizik – ochrana proti   >    >  [spamu.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="6a75c-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="6a75c-107">Pokud je **na kartě** Standardní povolené **standardní** nastavení, zaškrtněte seznamy **povolených** a **blokové seznamy.**</span><span class="sxs-lookup"><span data-stu-id="6a75c-107">On the **Standard** tab, if **Standard settings** is enabled, check the **Allow lists** and **Block lists**.</span></span>
3. <span data-ttu-id="6a75c-108">Pokud je **zapnuté**  vlastní nastavení, na kartě Vlastní  zkontrolujte zásady tak, že vyberete Upravit zásadu a zašepíšete seznamy **povolených** nebo **blokových seznamů.**</span><span class="sxs-lookup"><span data-stu-id="6a75c-108">On the **Custom** tab, if the **Custom settings** is enabled, review the policies by selecting **Edit policy** and checking the **Allow lists** and **Block lists**.</span></span>

<span data-ttu-id="6a75c-109">Další informace o konfiguraci zásad filtru spamu najdete v tématu Konfigurace zásad filtru [spamu.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="6a75c-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
