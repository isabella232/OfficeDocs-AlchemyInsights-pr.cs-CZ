---
title: Příklad zásady bezpečné přílohy v programu Microsoft Defender pro Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693103"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="60f97-102">Příklad zásady bezpečné přílohy v programu Microsoft Defender pro Office 365</span><span class="sxs-lookup"><span data-stu-id="60f97-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="60f97-103">Toto nastavení umožňuje zásadu s názvem *Bez* zpoždění, která zprávy hned doručí a potom znovu naskenuje přílohy:</span><span class="sxs-lookup"><span data-stu-id="60f97-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="60f97-104">**Název:** Bez zpoždění</span><span class="sxs-lookup"><span data-stu-id="60f97-104">**Name**: No delays</span></span>
- <span data-ttu-id="60f97-105">**Popis:** Zprávy se doručí okamžitě a znovu se naskenuje přílohy.</span><span class="sxs-lookup"><span data-stu-id="60f97-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="60f97-106">**Odpověď:** Vyberte možnost **dynamického doručení.**</span><span class="sxs-lookup"><span data-stu-id="60f97-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="60f97-107">Další informace najdete v článku [o dynamickém doručování v zásadách bezpečných příloh.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="60f97-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="60f97-108">**Část Přesměrovat** přílohu: Vyberte možnost povolit přesměrování a zadejte e-mailovou adresu globálního správce Microsoftu 365, správce zabezpečení nebo analytika zabezpečení, který bude prozkoumat škodlivé přílohy. </span><span class="sxs-lookup"><span data-stu-id="60f97-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="60f97-109">**Oddíl Použitý** na: **Vyberte doménu příjemce a** pak vyberte vaši doménu.</span><span class="sxs-lookup"><span data-stu-id="60f97-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="60f97-110">Vyberte **Přidat a** pak vyberte **OK.**</span><span class="sxs-lookup"><span data-stu-id="60f97-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="60f97-111">Až to budete mít, vyberte **Uložit.**</span><span class="sxs-lookup"><span data-stu-id="60f97-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="60f97-112">Další informace najdete v tématu Bezpečné [přílohy v programu Microsoft Defender pro Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="60f97-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
