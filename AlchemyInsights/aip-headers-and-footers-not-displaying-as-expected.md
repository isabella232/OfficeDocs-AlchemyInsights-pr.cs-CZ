---
title: 'AIP: Záhlaví a zápatí se nezobrazují podle očekávání'
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
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821692"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="25f8a-102">AIP: Záhlaví a zápatí se nezobrazují podle očekávání</span><span class="sxs-lookup"><span data-stu-id="25f8a-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="25f8a-103">Pokud máte problémy s vizuálními značkami, které se nezobrazují podle očekávání, podívejte se na následující pokyny:</span><span class="sxs-lookup"><span data-stu-id="25f8a-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="25f8a-104">Zkontrolujte, jestli jste si prohlédli [Při použití vizuálních znacích](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="25f8a-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="25f8a-105">Pokud chcete popisek Office označit, zkontrolujte, kdy [Office 365 používá označení a šifrování obsahu.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)</span><span class="sxs-lookup"><span data-stu-id="25f8a-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="25f8a-106">Pokud chcete odebrat existující záhlaví nebo zápatí, zkontrolujte Odebrání záhlaví a zápatí z jiných řešení [pro označování](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span><span class="sxs-lookup"><span data-stu-id="25f8a-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="25f8a-107">Pokud k tomuto problému stále dochází, shromážděte protokoly klienta Azure Information Protection a připojte exportované protokoly k tomuto lístku.</span><span class="sxs-lookup"><span data-stu-id="25f8a-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="25f8a-108">**Export protokolů Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="25f8a-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="25f8a-109">Otevřete dokument Office nebo vytvořte nový e-mail v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="25f8a-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="25f8a-110">Klikněte **na Zamknout/Citlivost**  >  **– nápověda a zpětná vazba.**</span><span class="sxs-lookup"><span data-stu-id="25f8a-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="25f8a-111">Klikněte **na Exportovat protokoly**.</span><span class="sxs-lookup"><span data-stu-id="25f8a-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="25f8a-112">Protokoly uložte do volby umístění a připojte je k této žádosti o službu.</span><span class="sxs-lookup"><span data-stu-id="25f8a-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="25f8a-113">Další informace najdete v těchto informacích:</span><span class="sxs-lookup"><span data-stu-id="25f8a-113">For additional information, see:</span></span>

- [<span data-ttu-id="25f8a-114">Jak nakonfigurovat popisek pro vizuální označení pro Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="25f8a-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="25f8a-115">Kontrola dokumentace k Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="25f8a-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="25f8a-116">Požadavky na Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="25f8a-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="25f8a-117">Úvodní kurz pro Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="25f8a-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="25f8a-118">Stažení klienta Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="25f8a-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
