---
title: Pravidlo ochrany před únikem čísla kreditní karty nefunguje
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679434"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="e7cab-102">Potíže s DLP s čísly kreditních karet</span><span class="sxs-lookup"><span data-stu-id="e7cab-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="e7cab-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e7cab-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e7cab-104">**Potíže s DLP s čísly kreditních karet**</span><span class="sxs-lookup"><span data-stu-id="e7cab-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="e7cab-105">Máte potíže s **zabráněním ztrátových dat (DLP)** , které nefungují u obsahu obsahujícího **číslo kreditní karty** v O365?</span><span class="sxs-lookup"><span data-stu-id="e7cab-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e7cab-106">Pokud ano, ujistěte se, že obsah obsahuje potřebné informace pro aktivaci zásady ochrany před únikem informací při vyhodnocování.</span><span class="sxs-lookup"><span data-stu-id="e7cab-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="e7cab-107">Například pro **zásady platební karty** , které jsou nakonfigurovány s úrovní spolehlivosti 85%, jsou vyhodnoceny následující vyhodnocení a musí být rozpoznáno, aby pravidlo aktivovalo:</span><span class="sxs-lookup"><span data-stu-id="e7cab-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e7cab-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, které je možné formátovat nebo Neformátovat (dddddddddddddddd) a které musí projít testem Luhn.</span><span class="sxs-lookup"><span data-stu-id="e7cab-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="e7cab-109">**[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Velmi složité a robustní vzorky, které zjišťují karty všech hlavních značek po celém světě, včetně VISA, MasterCard, karty Discover, JCB, American Express, dárkových poukazů a Diner karet.</span><span class="sxs-lookup"><span data-stu-id="e7cab-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="e7cab-110">**[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ano, kontrolní součet Luhn</span><span class="sxs-lookup"><span data-stu-id="e7cab-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="e7cab-111">**[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Zásada ochrany před únikem informací je 85%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:</span><span class="sxs-lookup"><span data-stu-id="e7cab-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e7cab-112">Funkce Func_credit_card najde obsah, který odpovídá vzoru.</span><span class="sxs-lookup"><span data-stu-id="e7cab-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e7cab-113">Je to pravda:</span><span class="sxs-lookup"><span data-stu-id="e7cab-113">One of the following is true:</span></span>

  - <span data-ttu-id="e7cab-114">Najde se klíčové slovo z Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="e7cab-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="e7cab-115">Najde se klíčové slovo z Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="e7cab-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="e7cab-116">Funkce Func_expiration_date najde datum ve správném formátu data.</span><span class="sxs-lookup"><span data-stu-id="e7cab-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="e7cab-117">Provedená kontrolní součty</span><span class="sxs-lookup"><span data-stu-id="e7cab-117">The checksum passes</span></span>

    <span data-ttu-id="e7cab-118">Například následující ukázka by mohla vyvolat zásadu pro nastavení čísel kreditní karty pro DLP:</span><span class="sxs-lookup"><span data-stu-id="e7cab-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="e7cab-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="e7cab-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="e7cab-120">Platnost vyprší: 2/2009</span><span class="sxs-lookup"><span data-stu-id="e7cab-120">Expires: 2/2009</span></span>

<span data-ttu-id="e7cab-121">Další informace o tom, co je potřeba pro zjištění **čísla kreditní karty** pro váš obsah, najdete v tomto článku v této části: [co citlivé typy informací vyhledají pro číslo kreditní karty #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="e7cab-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="e7cab-122">Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e7cab-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  