---
title: Oprava zásad připojení
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693302"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="3b346-102">Oprava zásad připojení</span><span class="sxs-lookup"><span data-stu-id="3b346-102">Fix connection policy</span></span>

<span data-ttu-id="3b346-103">E-mail byl označen jako bezpečný a doručený do složky doručené pošty uživatele, protože odesílající IP adresa byla v zásadách filtru připojení označená jako bezpečná.</span><span class="sxs-lookup"><span data-stu-id="3b346-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="3b346-104">Chcete-li tyto zásady zkontrolovat, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="3b346-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="3b346-105">Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143)potom přejděte na Zásady řízení rizik – ochrana proti   >    >  [spamu.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="3b346-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="3b346-106">Na kartě **Vlastní** vyberte zásadu filtru **připojení** a pak **vyberte Upravit zásadu.**</span><span class="sxs-lookup"><span data-stu-id="3b346-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="3b346-107">Zkontrolujte seznam **povolení PROTOKOLU IP.**</span><span class="sxs-lookup"><span data-stu-id="3b346-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="3b346-108">Podívejte **se, jestli je povolený** seznam bezpečných adres.</span><span class="sxs-lookup"><span data-stu-id="3b346-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3b346-109">Microsoft odebírá zdroje důvěryhodných odesílatelů od jiných výrobců.</span><span class="sxs-lookup"><span data-stu-id="3b346-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="3b346-110">Pokud **je povolený** seznam bezpečných adres, tito důvěryhodní odesílatelé se omylem označí jako spam.</span><span class="sxs-lookup"><span data-stu-id="3b346-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="3b346-111">Doporučujeme tuto možnost vybrat, protože se sníží počet falešně pozitivních zpráv (dobré zprávy, které jsou klasifikované jako spam), které dostanete.</span><span class="sxs-lookup"><span data-stu-id="3b346-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
