---
title: Oprava zásad tenanta (přepsání akce)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744477"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="41333-102">Oprava zásad tenanta (přepsání akce)</span><span class="sxs-lookup"><span data-stu-id="41333-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="41333-103">Tato zpráva se týká zásady ochrany proti spamu ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="41333-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="41333-104">Pokud chcete zásady zkontrolovat, proveďte toto:</span><span class="sxs-lookup"><span data-stu-id="41333-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="41333-105">Přejděte do [Centra zabezpečení Office 365 & Dodržování](https://go.microsoft.com/fwlink/p/?linkid=2077143)předpisů a pak přejděte na Zásady správy hrozeb   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="41333-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="41333-106">Zkontrolujte, jestli **zdroj zásad** označuje následující:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="41333-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="41333-107">Pokud ano, zkontrolujte na **kartě Vlastní** nastavení zásady, která zprávu ovlivnila.</span><span class="sxs-lookup"><span data-stu-id="41333-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="41333-108">Je možné, že  zpráva ovlivnila standardní nastavení použitá pro všechny zákazníky Exchange Online Protection.</span><span class="sxs-lookup"><span data-stu-id="41333-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="41333-109">Další informace o konfiguraci zásad filtru spamu najdete v tématu [Konfigurace zásad filtru spamu](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="41333-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
