---
title: Pravidlo ochrany před únikem číslo bankovního účtu USA nefunguje
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679289"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="c0ce4-102">Problémy s DLP s čísly bankovních účtů USA</span><span class="sxs-lookup"><span data-stu-id="c0ce4-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="c0ce4-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c0ce4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c0ce4-104">**Problémy s DLP s čísly bankovních účtů USA**</span><span class="sxs-lookup"><span data-stu-id="c0ce4-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="c0ce4-105">Máte problémy s funkcí ochrany před únikem informací **(DLP)** , která nefunguje u obsahu obsahujícího **číslo bankovního účtu USA** při používání informačního typu s citlivými informacemi o DLP v O365?</span><span class="sxs-lookup"><span data-stu-id="c0ce4-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c0ce4-106">Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co zásada ochrany před úniky hledá při vyhodnocování.</span><span class="sxs-lookup"><span data-stu-id="c0ce4-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c0ce4-107">Například pro zásady **bankovního účtu US** , která je nakonfigurovaná s úrovní spolehlivosti 85%, se vyhodnocuje následující hodnota, která se má pro pravidlo aktivovat:</span><span class="sxs-lookup"><span data-stu-id="c0ce4-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c0ce4-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 číslic</span><span class="sxs-lookup"><span data-stu-id="c0ce4-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="c0ce4-109">**[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 po sobě jdoucích číslic.</span><span class="sxs-lookup"><span data-stu-id="c0ce4-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="c0ce4-110">**[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, kontrolní součet neexistuje</span><span class="sxs-lookup"><span data-stu-id="c0ce4-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c0ce4-111">**[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zásada ochrany před únikem informací je 75%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:</span><span class="sxs-lookup"><span data-stu-id="c0ce4-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c0ce4-112">Regulární výraz Regex_usa_bank_account_number najde obsah, který odpovídá vzoru</span><span class="sxs-lookup"><span data-stu-id="c0ce4-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="c0ce4-113">Najde se klíčové slovo z Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="c0ce4-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="c0ce4-114">Například následující ukázka by aktivovala zásady **bankovního účtu USA** : kontrola účtu 78344011</span><span class="sxs-lookup"><span data-stu-id="c0ce4-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="c0ce4-115">Další informace o tom, co je potřeba pro zjištění **čísla bankovního účtu US** pro váš obsah, najdete v tomto článku v následující části: [co citlivé typy informací hledají číslo bankovního účtu USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .</span><span class="sxs-lookup"><span data-stu-id="c0ce4-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="c0ce4-116">Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c0ce4-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  