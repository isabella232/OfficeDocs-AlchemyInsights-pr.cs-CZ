---
title: 'AIP: Zásady se nechová podle očekávání'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821620"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="56fee-102">AIP: Zásady se nechová podle očekávání</span><span class="sxs-lookup"><span data-stu-id="56fee-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="56fee-103">Azure Information Protection: Zásady, které se nechová podle očekávání, najdete v následujících doporučených pokynech pro různé problémy se zásadami:</span><span class="sxs-lookup"><span data-stu-id="56fee-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="56fee-104">Pokud máte problémy s vizuálními značkami, přečtěte si prosím, kdy se [používají vizuální značky](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="56fee-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="56fee-105">Pokud máte problémy s automatickým označováním, přečtěte si prosím informace o tom, jak nakonfigurovat podmínky pro automatickou a doporučenou klasifikaci pro [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a Jaké typy citlivých informací [vypadají.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="56fee-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="56fee-106">Pokud máte problémy s ochranou Native/Pfile, přečtěte si prosím informace o [konfiguraci rozhraní API souboru](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="56fee-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="56fee-107">Zkontrolujte, jestli používáte zásady s oborem, které nejsou správně nakonfigurované: Jak nakonfigurovat zásady Azure Information Protection pro konkrétní uživatele pomocí [zásad s oborem](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="56fee-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="56fee-108">Pokud automatické označování nefunguje pro Outlook při připojování označeného dokumentu, ověřte, že funkce DRMEncryptProperty není definovaná podle popisu tady: Nastavení registru [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)pro zabezpečení .</span><span class="sxs-lookup"><span data-stu-id="56fee-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="56fee-109">Pokud máte pořád problémy, shromážděte protokoly klienta Azure Information Protection a připojte exportované protokoly k tomuto lístku.</span><span class="sxs-lookup"><span data-stu-id="56fee-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="56fee-110">Otevřete dokument Office nebo vytvořte nový e-mail v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="56fee-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="56fee-111">Klikněte **na Zamknout/Citlivost**  >  **– nápověda a zpětná vazba.**</span><span class="sxs-lookup"><span data-stu-id="56fee-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="56fee-112">Klikněte **na Exportovat protokoly**.</span><span class="sxs-lookup"><span data-stu-id="56fee-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="56fee-113">Protokoly uložte do volby umístění a připojte je k této žádosti o službu.</span><span class="sxs-lookup"><span data-stu-id="56fee-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="56fee-114">Další zdroje informací:</span><span class="sxs-lookup"><span data-stu-id="56fee-114">Additional resources:</span></span>

- [<span data-ttu-id="56fee-115">Jak nakonfigurovat popisek pro vizuální označení pro Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="56fee-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="56fee-116">Kontrola dokumentace k Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="56fee-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="56fee-117">Použití popisků citlivosti v aplikacích Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="56fee-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

