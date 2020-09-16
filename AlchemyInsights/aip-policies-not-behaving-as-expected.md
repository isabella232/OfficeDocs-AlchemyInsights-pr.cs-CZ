---
title: 'AIP: zásady se nechovají podle očekávání'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663182"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="9584c-102">AIP: zásady se nechovají podle očekávání</span><span class="sxs-lookup"><span data-stu-id="9584c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="9584c-103">Azure Information Protection: zásady nefungují podle očekávání, podívejte se na následující doporučení pro různé problémy se zásadami:</span><span class="sxs-lookup"><span data-stu-id="9584c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="9584c-104">Pokud máte problémy s vizuálními značkami, zkontrolujte, jestli [se vizuální značky používají](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="9584c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="9584c-105">Pokud máte problémy s automatickým popiskem, podívejte se [na článek Jak nakonfigurovat podmínky pro automatickou a doporučenou klasifikaci pro službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a [Jaké jsou tyto typy informací citlivé](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="9584c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="9584c-106">Pokud máte problémy s funkcí nativní/pfile Protection, zkontrolujte [konfiguraci rozhraní API souboru](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="9584c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="9584c-107">Zkontrolujte, jestli používáte zásady s oborem, které nejsou správně nakonfigurované: [jak nakonfigurovat zásady ochrany informací Azure pro určité uživatele pomocí zásad v oboru](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="9584c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="9584c-108">Pokud automatické připsání popisků nefunguje v Outlooku při připojování dokumentu označeného štítky, ověřte, že DRMEncryptProperty není definovaný, jak je popsáno tady: [nastavení registru IRM pro zabezpečení](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="9584c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="9584c-109">Pokud pořád dochází k problémům, Shromážděte protokoly klienta ochrany informací Azure a připojte k tomuto lístku exportované protokoly.</span><span class="sxs-lookup"><span data-stu-id="9584c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="9584c-110">Otevřete dokument Office nebo vytvořte nový e-mail v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="9584c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="9584c-111">Klikněte na **ochrana/citlivost**  >  **a váš názor**.</span><span class="sxs-lookup"><span data-stu-id="9584c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="9584c-112">Klikněte na **exportovat protokoly**.</span><span class="sxs-lookup"><span data-stu-id="9584c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="9584c-113">Protokoly uložte na svůj výběr a připojte je k tomuto požadavku služby.</span><span class="sxs-lookup"><span data-stu-id="9584c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="9584c-114">Další zdroje informací:</span><span class="sxs-lookup"><span data-stu-id="9584c-114">Additional resources:</span></span>

- [<span data-ttu-id="9584c-115">Jak nakonfigurovat popisek vizuálních značek pro Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9584c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="9584c-116">Přečtěte si dokumentaci k Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9584c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="9584c-117">Používání popisků citlivosti v aplikacích Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9584c-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

