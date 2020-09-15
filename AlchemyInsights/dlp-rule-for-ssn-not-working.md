---
title: Pravidlo ochrany před únikem pro SSN nefunguje
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679362"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="341fd-102">Problémy s DLP pomocí rodného čísla</span><span class="sxs-lookup"><span data-stu-id="341fd-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="341fd-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="341fd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="341fd-104">**Problémy s DLP v SSNs**</span><span class="sxs-lookup"><span data-stu-id="341fd-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="341fd-105">Máte problémy s funkcí ochrany před únikem informací **(DLP)** , která nefunguje u **Social Security Number (SSN)** obsahu obsahujícího důvěrné informace v Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="341fd-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="341fd-106">Pokud ano, ujistěte se, že váš obsah obsahuje potřebné informace o tom, co vypadá zásada ochrany před únikem informací.</span><span class="sxs-lookup"><span data-stu-id="341fd-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="341fd-107">Například zásady SSN, které jsou nakonfigurovány s úrovní spolehlivosti 85%, jsou vyhodnoceny a musí být detekovány, aby se pravidlo aktivovalo:</span><span class="sxs-lookup"><span data-stu-id="341fd-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="341fd-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, která mohou být ve formátu, který není naformátován</span><span class="sxs-lookup"><span data-stu-id="341fd-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="341fd-109">**[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Čtyři funkce hledejte SSNs ve čtyřech různých vzorcích:</span><span class="sxs-lookup"><span data-stu-id="341fd-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="341fd-110">Func_ssn najde SSNs 2011 s tučným formátováním, které je formátované pomocí pomlček nebo mezer (DDD-DD-dddd nebo DDD DD dddd).</span><span class="sxs-lookup"><span data-stu-id="341fd-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="341fd-111">Func_unformatted_ssn najde SSNs 2011 s neformátovaným silným formátováním (ddddddddd), které není formátované.</span><span class="sxs-lookup"><span data-stu-id="341fd-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="341fd-112">Func_randomized_formatted_ssn najde post-2011 SSNs, které jsou formátované pomocí pomlček nebo mezer (DDD-DD-dddd nebo DDD DD dddd).</span><span class="sxs-lookup"><span data-stu-id="341fd-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="341fd-113">Func_randomized_unformatted_ssn najde post-2011 SSNs, které nejsou formátované jako devět číslic za sebou (ddddddddd).</span><span class="sxs-lookup"><span data-stu-id="341fd-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="341fd-114">**[Kontrolní součet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, kontrolní součet neexistuje</span><span class="sxs-lookup"><span data-stu-id="341fd-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="341fd-115">**[Definice:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Zásada ochrany před únikem informací je 85%, že se tento typ citlivých informací zjistil, pokud v blízkosti 300 znaků:</span><span class="sxs-lookup"><span data-stu-id="341fd-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="341fd-116">[Funkce Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) najde obsah, který odpovídá vzoru.</span><span class="sxs-lookup"><span data-stu-id="341fd-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="341fd-117">Najde se klíčové slovo z [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="341fd-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="341fd-118">Mezi příklady klíčových slov patří:  *sociální zabezpečení, sociálního zabezpečení #, SOC s, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="341fd-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="341fd-119">Například následující ukázka by mohla vyvolat zásadu ochrany před DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="341fd-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="341fd-120">Další informace o tom, co je potřeba pro SSNs pro váš obsah, najdete v tomto článku v následující části: [co citlivé typy informací budou hledat pro SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) .</span><span class="sxs-lookup"><span data-stu-id="341fd-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="341fd-121">Pomocí jiného integrovaného typu citlivých informací najdete v následujícím článku informace o tom, co je potřeba pro jiné typy: [Jaké mají citlivé typy informací](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="341fd-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  