---
title: Tipy zásad ochrany před únikem informací nefungují
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958695"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="ea322-102">Problémy s tipy pro zásady ochrany před únikem informací</span><span class="sxs-lookup"><span data-stu-id="ea322-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="ea322-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ea322-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ea322-104">Pokud chcete nakonfigurovat tipy zásad pro zásady ochrany před únikem informací v Centru & dodržování předpisů v úplném režimu vynucení, proveďte toto:</span><span class="sxs-lookup"><span data-stu-id="ea322-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="ea322-105">Zajistěte, aby byly u pravidla DLP **povolené** tipy zásad.</span><span class="sxs-lookup"><span data-stu-id="ea322-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="ea322-106">Postup najdete v tématu [Odesílání e-mailových oznámení a zobrazení tipů zásad pro zásady ochrany před únikem informací](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="ea322-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="ea322-107">Zajistěte, aby váš obsah odpovídal tomu, co je potřeba k aktivaci pravidla popsaného v [definicích](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)entit typu Citlivé informace .</span><span class="sxs-lookup"><span data-stu-id="ea322-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="ea322-108">Tipy pro zásady se zobrazují v aplikaci OWA i v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="ea322-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="ea322-109">Při používání Outlooku 2013 nebo novějšího se ale tipy zásad zobrazují jenom za určitých podmínek.</span><span class="sxs-lookup"><span data-stu-id="ea322-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="ea322-110">Seznam konkrétních podmínek najdete v tématu [Podporované podmínky pro Outlook 2013 nebo novější](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)pro zobrazení tipů zásad .</span><span class="sxs-lookup"><span data-stu-id="ea322-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="ea322-111">Informace o tipech zásad ochrany před únikem informací najdete v tématu Tipy pro zásady [ochrany před](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) únikem informací – referenční informace a matice podpory pro tipy zásad ochrany před únikem [informací](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span><span class="sxs-lookup"><span data-stu-id="ea322-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>