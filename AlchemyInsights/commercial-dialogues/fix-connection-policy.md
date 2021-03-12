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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744849"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="e5861-102">Oprava zásad připojení</span><span class="sxs-lookup"><span data-stu-id="e5861-102">Fix connection policy</span></span>

<span data-ttu-id="e5861-103">E-mail byl označený jako bezpečný a doručený do složky Doručená pošta uživatele, protože odesílající IP adresa byla v zásadách filtru připojení označená jako bezpečná.</span><span class="sxs-lookup"><span data-stu-id="e5861-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="e5861-104">Pokud chcete zásady zkontrolovat, proveďte toto:</span><span class="sxs-lookup"><span data-stu-id="e5861-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="e5861-105">Přejděte do [Centra zabezpečení Office 365 & Dodržování](https://go.microsoft.com/fwlink/p/?linkid=2077143)předpisů a pak přejděte na Zásady správy hrozeb   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="e5861-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="e5861-106">Na kartě **Vlastní** vyberte zásadu **filtru** Připojení a pak vyberte **Upravit zásadu.**</span><span class="sxs-lookup"><span data-stu-id="e5861-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="e5861-107">Zkontrolujte seznam **POVOLIT IP** adres.</span><span class="sxs-lookup"><span data-stu-id="e5861-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="e5861-108">Podívejte se, **jestli je povolený** bezpečný seznam.</span><span class="sxs-lookup"><span data-stu-id="e5861-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e5861-109">Microsoft si předplatí zdroje důvěryhodných odesílatelů třetích stran.</span><span class="sxs-lookup"><span data-stu-id="e5861-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="e5861-110">Pokud **je povolený** bezpečný seznam, tito důvěryhodní odesílatelé se omylem označí jako spam.</span><span class="sxs-lookup"><span data-stu-id="e5861-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="e5861-111">Tuto možnost doporučujeme vybrat, protože se tím sníží počet falešně pozitivních zpráv (dobrá pošta, která je klasifikovaná jako spam), kterou dostanete.</span><span class="sxs-lookup"><span data-stu-id="e5861-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
