---
title: Pravidlo ochrany před únikem pro číslo účtu USA/UK nefunguje
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679217"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="9bd36-102">Problémy s DLP – čísla v USA/ČR Passport</span><span class="sxs-lookup"><span data-stu-id="9bd36-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="9bd36-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="9bd36-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9bd36-104">**Problémy s DLP v USA/Spojeném účtu Passport**</span><span class="sxs-lookup"><span data-stu-id="9bd36-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="9bd36-105">Máte problémy s funkcí ochrany před únikem informací **(DLP)** , která nefunguje u obsahu obsahujícího v systému O365 informační typ s informacemi o tom, že je k dispozici v **USA/Spojeném** ?</span><span class="sxs-lookup"><span data-stu-id="9bd36-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="9bd36-106">Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co zásada ochrany před úniky hledá při vyhodnocování.</span><span class="sxs-lookup"><span data-stu-id="9bd36-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="9bd36-107">Například pro zásady **čísla cestovního pasu pro USA/spojené** s úrovní spolehlivosti 75% jsou následující vyhodnoceny a musí být detekovány, aby se pravidlo spouštěly.</span><span class="sxs-lookup"><span data-stu-id="9bd36-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="9bd36-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devět číslic</span><span class="sxs-lookup"><span data-stu-id="9bd36-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="9bd36-109">**[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devět po sobě jdoucích číslic</span><span class="sxs-lookup"><span data-stu-id="9bd36-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="9bd36-110">**[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, kontrolní součet neexistuje</span><span class="sxs-lookup"><span data-stu-id="9bd36-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="9bd36-111">**[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Zásada ochrany před únikem informací je 75%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:</span><span class="sxs-lookup"><span data-stu-id="9bd36-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9bd36-112">Funkce Func_usa_uk_passport najde obsah, který odpovídá vzoru.</span><span class="sxs-lookup"><span data-stu-id="9bd36-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="9bd36-113">Najde se klíčové slovo z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="9bd36-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="9bd36-114">Například následující ukázka by mohla vyvolat zásadu **čísla pasu USA/UK** : číslo USA 123456789</span><span class="sxs-lookup"><span data-stu-id="9bd36-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="9bd36-115">Další informace o tom, co je potřeba pro zjištění čísla US/UK pro váš obsah, najdete v tomto článku v této části: [Jaké jsou typy citlivých informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .</span><span class="sxs-lookup"><span data-stu-id="9bd36-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="9bd36-116">Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="9bd36-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  