---
title: DLP může potřebovat vlastní typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712177"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="89c09-102">DLP může potřebovat vlastní typ</span><span class="sxs-lookup"><span data-stu-id="89c09-102">DLP might need a custom type</span></span>

<span data-ttu-id="89c09-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="89c09-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="89c09-104">**DLP může vyžadovat vlastní typ informací.**</span><span class="sxs-lookup"><span data-stu-id="89c09-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="89c09-105">Pomocí zásad ochrany před únikem informací můžete identifikovat a chránit citlivá data ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="89c09-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="89c09-106">V některých scénářích budete muset **vytvořit vlastní typ citlivých** informací, abyste chránili data organizace.</span><span class="sxs-lookup"><span data-stu-id="89c09-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="89c09-107">Vaše organizace může například potřebovat identifikovat a chránit ID zaměstnanců nebo jiná data v některém formátu určeném pro vaši organizaci. Pokud ano, najdete další informace v následujících článcích.</span><span class="sxs-lookup"><span data-stu-id="89c09-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="89c09-108">**Přizpůsobení předdefinovaného citlivého typu informací**</span><span class="sxs-lookup"><span data-stu-id="89c09-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="89c09-109">Pokud by integrovaný typ citlivých informací splňoval vaše potřeby jenom s několika vylepšeními, můžete [přizpůsobit integrovaný typ citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="89c09-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="89c09-110">Můžete například přidat nebo odebrat klíčová slova nebo přidat nebo odebrat podpůrný důkaz, například datum nebo adresu.</span><span class="sxs-lookup"><span data-stu-id="89c09-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="89c09-111">**Vytvoření vlastního typu citlivých informací**</span><span class="sxs-lookup"><span data-stu-id="89c09-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="89c09-112">Pokud ale potřebujete zjistit a chránit jiný typ citlivých informací, můžete [vytvořit vlastní typ citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) v uživatelském rozhraní centra zabezpečení &.</span><span class="sxs-lookup"><span data-stu-id="89c09-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="89c09-113">**Vytvoření vlastního typu citlivých informací v prostředí PowerShell centra dodržování předpisů &**</span><span class="sxs-lookup"><span data-stu-id="89c09-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="89c09-114">Pokud uživatelské rozhraní nenabízí všechny možnosti, které potřebujete, můžete si [vytvořit vlastní typ citlivých informací v prostředí PowerShell centra dodržování předpisů &](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="89c09-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="89c09-115">Spuštěním souboru XML můžete použít všechny dostupné možnosti.</span><span class="sxs-lookup"><span data-stu-id="89c09-115">By starting with an XML file, you can use every option available.</span></span>
