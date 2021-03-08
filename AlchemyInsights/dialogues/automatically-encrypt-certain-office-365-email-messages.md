---
title: Automatické šifrování některých e-mailových zpráv Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524010"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="dc193-102">Automatické šifrování některých e-mailových zpráv Office 365</span><span class="sxs-lookup"><span data-stu-id="dc193-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="dc193-103">Zprávy, které uživatelé pošlou určitým externím lidem nebo organizacím, můžete automaticky šifrovat.</span><span class="sxs-lookup"><span data-stu-id="dc193-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="dc193-104">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="dc193-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="dc193-105">V Centru [pro správu Exchange zvolte](https://outlook.office365.com/ecp/) **tok pošty a > pravidla.**</span><span class="sxs-lookup"><span data-stu-id="dc193-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="dc193-106">Klikněte na **ikonu Nový (+)** a potom klikněte na Použít šifrování zpráv **Office 365 a ochranu přístupových práv u zpráv.**</span><span class="sxs-lookup"><span data-stu-id="dc193-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="dc193-107">Do **pole** Název zadejte název pravidla, například Šifrování zpráv odeslaných *DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="dc193-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="dc193-108">V **části Použít toto pravidlo vyberte** Příjemce, > je tato **osoba.**</span><span class="sxs-lookup"><span data-stu-id="dc193-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="dc193-109">V okně **Vybrat členy** vyberte jméno osoby, na kterou chcete pravidlo šifrování použít, a klikněte na **Přidat.**</span><span class="sxs-lookup"><span data-stu-id="dc193-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="dc193-110">Po přidání uživatelů klikněte na **OK.**</span><span class="sxs-lookup"><span data-stu-id="dc193-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="dc193-111">Vedle pole **Provést následující klikněte** na Vybrat jednu z **nich.**</span><span class="sxs-lookup"><span data-stu-id="dc193-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="dc193-112">V rozevírací **nabídce šablony RMS** vyberte **Šifrovat** a potom klikněte na **OK.**</span><span class="sxs-lookup"><span data-stu-id="dc193-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="dc193-113">(Pokud tuto možnost nevidíte, znamená to, že váš plán nezahrnuje automatické šifrování.</span><span class="sxs-lookup"><span data-stu-id="dc193-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="dc193-114">Můžete ho ale přidat!)</span><span class="sxs-lookup"><span data-stu-id="dc193-114">But you can add it!)</span></span>
9. <span data-ttu-id="dc193-115">Zvolte libovolný volitelný výběr (ze seznamu volitelných výběrů, které můžete v tomto okamžiku provést, z nichž mnohé mohou být ponechány s výchozím nastavením pro jednoduchost).</span><span class="sxs-lookup"><span data-stu-id="dc193-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="dc193-116">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="dc193-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="dc193-117">Toto pravidlo můžete později zase vrátit a upravit.</span><span class="sxs-lookup"><span data-stu-id="dc193-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="dc193-118">Další informace o vytváření pravidel pro šifrování najdete v článku Definice pravidel toku pošty pro šifrování e-mailových zpráv v [Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="dc193-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

