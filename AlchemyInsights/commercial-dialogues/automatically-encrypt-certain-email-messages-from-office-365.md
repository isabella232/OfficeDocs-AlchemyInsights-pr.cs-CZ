---
title: Automatické šifrování určitých e-mailových zpráv z Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744585"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="f31c1-102">Automatické šifrování určitých e-mailových zpráv z Office 365</span><span class="sxs-lookup"><span data-stu-id="f31c1-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="f31c1-103">V Centru [pro správu Exchange](https://outlook.office365.com/ecp/)zvolte **tok pošty > pravidla**.</span><span class="sxs-lookup"><span data-stu-id="f31c1-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="f31c1-104">Klikněte na **ikonu Nový (+)** a potom klikněte na Použít šifrování zpráv **Office 365** a ochranu práv u zpráv.</span><span class="sxs-lookup"><span data-stu-id="f31c1-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="f31c1-105">Do **pole** Název zadejte název pravidla, například *Zašifrovat všechny zprávy*.</span><span class="sxs-lookup"><span data-stu-id="f31c1-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="f31c1-106">V **části Použít toto pravidlo, pokud** zvolte **[Použít u všech zpráv]**.</span><span class="sxs-lookup"><span data-stu-id="f31c1-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="f31c1-107">Vedle pole **Do the following (Provést následující)** klikněte na Select one **(Vybrat jednu).**</span><span class="sxs-lookup"><span data-stu-id="f31c1-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="f31c1-108">V rozevírací **nabídce šablony RMS** vyberte Šifrovat a potom klikněte na **OK.** </span><span class="sxs-lookup"><span data-stu-id="f31c1-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="f31c1-109">(Pokud tuto možnost nevidíte, znamená to, že váš plán neobsahuje automatické šifrování.</span><span class="sxs-lookup"><span data-stu-id="f31c1-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="f31c1-110">Ale můžete ho přidat!)</span><span class="sxs-lookup"><span data-stu-id="f31c1-110">But you can add it!)</span></span>
7. <span data-ttu-id="f31c1-111">Zaškrtněte políčko **Auditovat toto pravidlo s úrovní závažnosti** a pak vyberte požadovanou úroveň.</span><span class="sxs-lookup"><span data-stu-id="f31c1-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="f31c1-112">Pokud má vaše společnost smluvní závazky posílat všechny e-maily zašifrované, doporučujeme nastavit úroveň **Vysoká.**</span><span class="sxs-lookup"><span data-stu-id="f31c1-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="f31c1-113">V **části Zvolit model pro toto pravidlo** klikněte na **Vynutit**.</span><span class="sxs-lookup"><span data-stu-id="f31c1-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="f31c1-114">Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé můžete nechat s výchozím nastavením pro jednoduchost).</span><span class="sxs-lookup"><span data-stu-id="f31c1-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="f31c1-115">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="f31c1-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f31c1-116">Toto pravidlo se můžete vrátit a toto pravidlo upravit později.</span><span class="sxs-lookup"><span data-stu-id="f31c1-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="f31c1-117">Další informace o vytváření pravidel pro šifrování najdete v článku Definování pravidel toku pošty pro šifrování e-mailových zpráv [v Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="f31c1-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

