---
title: Příklad zásad bezpečné přílohy v Programu Microsoft Defender pro Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744525"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="6ec96-102">Příklad zásad bezpečné přílohy v Programu Microsoft Defender pro Office 365</span><span class="sxs-lookup"><span data-stu-id="6ec96-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="6ec96-103">Tato nastavení povolte zásadu *s* názvem Žádná zpoždění, která okamžitě doručí zprávy, a potom přílohy znovu připojte po jejich naskenování:</span><span class="sxs-lookup"><span data-stu-id="6ec96-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="6ec96-104">**Název:** Bez zpoždění</span><span class="sxs-lookup"><span data-stu-id="6ec96-104">**Name**: No delays</span></span>
- <span data-ttu-id="6ec96-105">**Popis:** Doručuje zprávy okamžitě a znovu přichytá přílohy po skenování.</span><span class="sxs-lookup"><span data-stu-id="6ec96-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="6ec96-106">**Odpověď:** Vyberte **možnost Dynamické doručení.**</span><span class="sxs-lookup"><span data-stu-id="6ec96-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="6ec96-107">Další informace najdete v tématu [Dynamické doručování v zásadách bezpečných příloh](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="6ec96-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="6ec96-108">**Oddíl Příloha přesměrování:** Vyberte možnost Povolit přesměrování a zadejte e-mailovou adresu globálního správce Microsoftu 365, správce zabezpečení nebo analytika zabezpečení, který bude zkoumat škodlivé přílohy.</span><span class="sxs-lookup"><span data-stu-id="6ec96-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="6ec96-109">**Oddíl Použitý na:** Vyberte **Doména příjemce je** a pak vyberte doménu.</span><span class="sxs-lookup"><span data-stu-id="6ec96-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="6ec96-110">Vyberte **přidat** a pak vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="6ec96-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="6ec96-111">Po dokončení vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="6ec96-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="6ec96-112">Další informace najdete v tématu [Bezpečné přílohy v programu Microsoft Defender pro Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="6ec96-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
