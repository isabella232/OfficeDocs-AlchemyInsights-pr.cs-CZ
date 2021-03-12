---
title: DLP nefunguje podle očekávání
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707803"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="aac2f-102">DLP nefunguje podle očekávání</span><span class="sxs-lookup"><span data-stu-id="aac2f-102">DLP not working as expected</span></span>

<span data-ttu-id="aac2f-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="aac2f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="aac2f-104">**Nastavení DLP**</span><span class="sxs-lookup"><span data-stu-id="aac2f-104">**Setting up DLP**</span></span>

<span data-ttu-id="aac2f-105">Máte problémy s prevencí ztráty dat **(DLP)** v Office 365, která nefunguje podle očekávání?</span><span class="sxs-lookup"><span data-stu-id="aac2f-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="aac2f-106">Pokud ano, ujistěte  se, že máte správně nastavenou zásadu  ochrany před únikem informací a jestli data obsahují to, co zásada ochrany před únikem informací hledá při vyhodnocení.</span><span class="sxs-lookup"><span data-stu-id="aac2f-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="aac2f-107">Zásady ochrany před únikem informací umožňují identifikovat a chránit citlivé informace ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="aac2f-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="aac2f-108">Pokud chcete nastavit zásady ochrany před únikem informací, použijte [informace uvedené v této článku.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="aac2f-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="aac2f-109">**Jaké zásady ochrany před únikem informací hledat**</span><span class="sxs-lookup"><span data-stu-id="aac2f-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="aac2f-110">Při používání **integrovaných** citlivých typů informací v centrech zabezpečení a dodržování předpisů zásady ochrany před únikem informací při zjišťování těchto citlivých typů zjišťují konkrétní vzory a prvky.</span><span class="sxs-lookup"><span data-stu-id="aac2f-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="aac2f-111">**Integrované citlivé typy informací**</span><span class="sxs-lookup"><span data-stu-id="aac2f-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="aac2f-112">Informace o předdefinových typech s citlivými typy a o tom, co zásady ochrany před únikem informací hledá při zjišťování typu citlivé informace, najdete v tématu: Co citlivé typy [informací vyhledáte.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="aac2f-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="aac2f-113">**Vlastní citlivé typy informací**</span><span class="sxs-lookup"><span data-stu-id="aac2f-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="aac2f-114">Pokud se pokoušíte vytvořit vlastní citlivé typy informací, použijte v následujícím článku informace o vytvoření vlastního citlivého typu: Vytvoření vlastního typu citlivé [informace.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="aac2f-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="aac2f-115">**Testování zásad ochrany před únikem informací**</span><span class="sxs-lookup"><span data-stu-id="aac2f-115">**Test a DLP policy**</span></span>

<span data-ttu-id="aac2f-116">Pokud chcete data testovat pomocí předdefinového nebo vlastního citlivého typu informací, použijte možnost **Typ** testu v části Typy informací citlivé  >  **na klasifikace.**</span><span class="sxs-lookup"><span data-stu-id="aac2f-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="aac2f-117">Další informace najdete v tématu [Testování vlastních citlivých typů informací.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="aac2f-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="aac2f-118">**Sestavy**</span><span class="sxs-lookup"><span data-stu-id="aac2f-118">**Reports**</span></span>
  
- <span data-ttu-id="aac2f-119">Díky sestavám ochrany před únikem informací získáte citlivé [poznatky o datech.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="aac2f-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="aac2f-120">Podívejte se na konkrétní podrobnosti o události se [zprávou o incidentu.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="aac2f-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
