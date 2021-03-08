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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524014"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="4fa68-102">Automatické šifrování určitých e-mailových zpráv z Office 365</span><span class="sxs-lookup"><span data-stu-id="4fa68-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="4fa68-103">V Centru [pro správu Exchange zvolte](https://outlook.office365.com/ecp/) **tok pošty a > pravidla.**</span><span class="sxs-lookup"><span data-stu-id="4fa68-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="4fa68-104">Klikněte na **ikonu Nový (+)** a potom klikněte na Použít šifrování zpráv **Office 365 a ochranu přístupových práv u zpráv.**</span><span class="sxs-lookup"><span data-stu-id="4fa68-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="4fa68-105">Do **pole** Název zadejte název pravidla, například Zašifrovat *všechny zprávy.*</span><span class="sxs-lookup"><span data-stu-id="4fa68-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="4fa68-106">V **části Použít toto pravidlo zvolte** **[Použít u všech zpráv]**.</span><span class="sxs-lookup"><span data-stu-id="4fa68-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="4fa68-107">Vedle pole **Provést následující klikněte** na Vybrat jednu z **nich.**</span><span class="sxs-lookup"><span data-stu-id="4fa68-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="4fa68-108">V rozevírací **nabídce šablony RMS** vyberte **Šifrovat** a potom klikněte na **OK.**</span><span class="sxs-lookup"><span data-stu-id="4fa68-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="4fa68-109">(Pokud tuto možnost nevidíte, znamená to, že váš plán nezahrnuje automatické šifrování.</span><span class="sxs-lookup"><span data-stu-id="4fa68-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="4fa68-110">Můžete ho ale přidat!)</span><span class="sxs-lookup"><span data-stu-id="4fa68-110">But you can add it!)</span></span>
7. <span data-ttu-id="4fa68-111">Zaškrtněte políčko **Auditovat toto pravidlo s** úrovní závažnosti a vyberte požadovanou úroveň.</span><span class="sxs-lookup"><span data-stu-id="4fa68-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="4fa68-112">Pokud má vaše společnost smluvní povinnosti, aby se odesílali všechny e-maily zašifrované, doporučujeme nastavit úroveň **na Vysokou.**</span><span class="sxs-lookup"><span data-stu-id="4fa68-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="4fa68-113">V **části Zvolte model pro toto pravidlo** klikněte na **Vynutit.**</span><span class="sxs-lookup"><span data-stu-id="4fa68-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="4fa68-114">Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé mohou být ponechány s výchozím nastavením pro jednoduchost).</span><span class="sxs-lookup"><span data-stu-id="4fa68-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="4fa68-115">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="4fa68-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4fa68-116">Toto pravidlo můžete později zase vrátit a upravit.</span><span class="sxs-lookup"><span data-stu-id="4fa68-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="4fa68-117">Další informace o vytváření pravidel pro šifrování najdete v článku Definice pravidel toku pošty pro šifrování e-mailových zpráv v [Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="4fa68-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

