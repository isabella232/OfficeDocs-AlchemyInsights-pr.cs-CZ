---
title: Nefungují tipy pro zásady DLP
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
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679578"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="c334f-102">Problémy s tipem na ochranu před únikem informací</span><span class="sxs-lookup"><span data-stu-id="c334f-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="c334f-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c334f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c334f-104">**Tipy pro zásady DLP**</span><span class="sxs-lookup"><span data-stu-id="c334f-104">**DLP policy tips**</span></span>

<span data-ttu-id="c334f-105">Při použití **zásad ochrany před únikem informací**mohou uživatelé upozorňovat na porušení zásad pomocí **tipů zásad**.</span><span class="sxs-lookup"><span data-stu-id="c334f-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="c334f-106">Správci můžou nakonfigurovat tipy zásad, aby se zobrazovaly při testování jejich zásad ochrany před únikem informací nebo když je zásada v plném režimu vynucení.</span><span class="sxs-lookup"><span data-stu-id="c334f-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="c334f-107">Pokud chcete nakonfigurovat tipy zásad pro zásady ochrany před únikem informací v centru zabezpečení a dodržování předpisů v režimu úplného vynucení, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="c334f-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="c334f-108">Zkontrolujte, jestli jsou v pravidle o DLP **zapnuté** tyto pokyny [.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="c334f-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="c334f-109">Zajistěte, aby váš **obsah odpovídal** tomu, co je **potřeba** k aktivaci pravidla popsaného v [tomto článku.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c334f-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="c334f-110">Tipy zásad se zobrazují v OWA i Outlooku.</span><span class="sxs-lookup"><span data-stu-id="c334f-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="c334f-111">Když ale používáte **Outlook 2013 nebo novější**, zobrazí se tipy zásad pouze za určitých podmínek.</span><span class="sxs-lookup"><span data-stu-id="c334f-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="c334f-112">Tady jsou uvedené podmínky: [podporované podmínky pro Outlook 2013 nebo novější pro zobrazení tipů zásad](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="c334f-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="c334f-113">Další informace o tipech zásad ochrany před únikem informací najdete v tématu [Zobrazení tipů zásad pro zásady ochrany před únikem](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips) .</span><span class="sxs-lookup"><span data-stu-id="c334f-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  