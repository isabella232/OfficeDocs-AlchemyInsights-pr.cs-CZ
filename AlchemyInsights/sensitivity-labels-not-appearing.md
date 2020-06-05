---
title: Popisky citlivosti se nezobrazují
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581008"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="3f9c7-102">Popisky citlivosti se nezobrazují</span><span class="sxs-lookup"><span data-stu-id="3f9c7-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="3f9c7-103">Popisky citlivosti umožňují klasifikovat a chránit citlivý obsah.</span><span class="sxs-lookup"><span data-stu-id="3f9c7-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="3f9c7-104">Mohou být vytvořeny v Centru dodržování předpisů Microsoft 365, Microsoft 365 Security Center nebo Microsoft 365 Security & Compliance Center v rámci popisků klasifikace > citlivosti.</span><span class="sxs-lookup"><span data-stu-id="3f9c7-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="3f9c7-105">Další informace o této funkci naleznete v [tématu Přehled popisků citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="3f9c7-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="3f9c7-106">Pokud jste nakonfigurovali štítky citlivosti, ale nezobrazují se v aplikacích Microsoft 365, zkontrolujte následující:</span><span class="sxs-lookup"><span data-stu-id="3f9c7-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="3f9c7-107">Zkontrolujte, zda byl popisek [citlivosti publikován](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) uživatelům a požadovaným skupinám.</span><span class="sxs-lookup"><span data-stu-id="3f9c7-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="3f9c7-108">Zkontrolujte, zda uživatel používá aplikaci, která podporuje popisky citlivosti – [viz popisky citlivosti v dokumentu](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="3f9c7-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="3f9c7-109">Pokud [migrujete popisky Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), mějte na paměti zde [uvedené](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)důležité informace .</span><span class="sxs-lookup"><span data-stu-id="3f9c7-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="3f9c7-110">Podpora ochrany před únikem informací (DLP): V současné době lze jako podmínku v zásadách ochrany před únikem informací použít jako podmínku pouze popisky uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="3f9c7-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="3f9c7-111">Podpora popisků citlivosti v zásadách ochrany před únikem dat ještě není k dispozici, ale pracujeme na ní.</span><span class="sxs-lookup"><span data-stu-id="3f9c7-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="3f9c7-112">Pokud je šifrování povoleno na štítku citlivosti, můžete zvolit:</span><span class="sxs-lookup"><span data-stu-id="3f9c7-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="3f9c7-113">Přiřazovat oprávnění</span><span class="sxs-lookup"><span data-stu-id="3f9c7-113">Assign permissions now</span></span>
    - <span data-ttu-id="3f9c7-114">Povolit uživatelům přiřazovat oprávnění</span><span class="sxs-lookup"><span data-stu-id="3f9c7-114">Let users assign permissions</span></span>


<span data-ttu-id="3f9c7-115">Další informace o možných problémech naleznete v [tématu Známé problémy s popisky citlivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="3f9c7-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>