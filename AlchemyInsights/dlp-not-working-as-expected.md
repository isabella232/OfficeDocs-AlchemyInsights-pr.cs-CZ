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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679686"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="311d4-102">DLP nefunguje podle očekávání</span><span class="sxs-lookup"><span data-stu-id="311d4-102">DLP not working as expected</span></span>

<span data-ttu-id="311d4-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="311d4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="311d4-104">**Nastavení DLP**</span><span class="sxs-lookup"><span data-stu-id="311d4-104">**Setting up DLP**</span></span>

<span data-ttu-id="311d4-105">Máte potíže s **zabráněním ochrany dat (DLP)** v Office 365 nefunguje podle očekávání?</span><span class="sxs-lookup"><span data-stu-id="311d4-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="311d4-106">Pokud ano, ujistěte se, že máte správně nastavené **Zásady ochrany před únikem informací** a že vaše data obsahují informace o tom, co při vyhodnocování **Zásada ochrany před úniky** hledá.</span><span class="sxs-lookup"><span data-stu-id="311d4-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="311d4-107">Zásady ochrany před únikem umožňuje identifikovat a chránit citlivé informace ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="311d4-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="311d4-108">K nastavení zásad ochrany před únikem informací použijte [tyto informace.](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="311d4-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="311d4-109">**Co vyhledává zásady ochrany před únikem**</span><span class="sxs-lookup"><span data-stu-id="311d4-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="311d4-110">Při používání **vestavěných citlivých informací** v centru zabezpečení a dodržování předpisů vyhledává zásady pro DLP při zjišťování těchto citlivých typů určité vzorky a prvky.</span><span class="sxs-lookup"><span data-stu-id="311d4-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="311d4-111">**Předdefinované citlivé typy informací**</span><span class="sxs-lookup"><span data-stu-id="311d4-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="311d4-112">Informace o vestavěných citlivých typech a o tom, co zásada ochrany před úniky hledá při zjišťování citlivého typu, najdete v tématu: [Jaké typy citlivých informací vypadají](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="311d4-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="311d4-113">**Vlastní typy citlivých informací**</span><span class="sxs-lookup"><span data-stu-id="311d4-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="311d4-114">Pokud chcete vytvořit vlastní typy citlivých informací, použijte následující článek, kde najdete informace o tom, jak vytvořit vlastní typ citlivých informací: [Vytvořte si vlastní typ citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="311d4-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="311d4-115">**Testování zásad ochrany před únikem informací**</span><span class="sxs-lookup"><span data-stu-id="311d4-115">**Test a DLP policy**</span></span>

<span data-ttu-id="311d4-116">Chcete-li testovat data pomocí předdefinovaných nebo vlastních typů citlivých informací, použijte možnost **Typ testu** **v části**  >  **typy utajovaných informací**.</span><span class="sxs-lookup"><span data-stu-id="311d4-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="311d4-117">Další informace najdete v článku [testování vlastních typů citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="311d4-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="311d4-118">**Sestavy**</span><span class="sxs-lookup"><span data-stu-id="311d4-118">**Reports**</span></span>
  
- <span data-ttu-id="311d4-119">Získejte citlivé datové přehledy s informacemi o [DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="311d4-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="311d4-120">Podívejte se na určité podrobnosti o události se [sestavou incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="311d4-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
