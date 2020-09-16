---
title: Nezobrazují se popisky citlivosti
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801177"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="3aa25-102">Nezobrazují se popisky citlivosti</span><span class="sxs-lookup"><span data-stu-id="3aa25-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="3aa25-103">Popisky citlivosti umožňují klasifikovat a chránit váš citlivý obsah.</span><span class="sxs-lookup"><span data-stu-id="3aa25-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="3aa25-104">Lze je vytvořit v centru dodržování předpisů v systému Microsoft 365, v centru zabezpečení Microsoft 365 nebo v centru & zabezpečení Microsoft 365 pod nadpisy > hodnocení.</span><span class="sxs-lookup"><span data-stu-id="3aa25-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="3aa25-105">Další informace o této funkci najdete v tématu [Přehled popisů citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="3aa25-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="3aa25-106">Pokud jste své popisky citlivosti nakonfigurovali, ale nevidíte v aplikacích Microsoft 365, podívejte se na tyto skutečnosti:</span><span class="sxs-lookup"><span data-stu-id="3aa25-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="3aa25-107">Ověřte, že popisek citlivosti [publikovaný](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) pro požadované uživatele a skupiny.</span><span class="sxs-lookup"><span data-stu-id="3aa25-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="3aa25-108">Potvrďte, že uživatel používá aplikaci, která podporuje popisky citlivosti – Podívejte [se na popisky citlivosti v dokumentu](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="3aa25-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="3aa25-109">Pokud [migrujete štítky ochrany informací Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), uvědomte si, jaké jsou [tu tady](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="3aa25-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="3aa25-110">Podpora ochrany před únikem informací: v zásadách ochrany před úniky v současné době mohou být použity pouze štítky pro uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="3aa25-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="3aa25-111">Podpora štítků s citlivostí v zásadách ochrany před úniky ještě není k dispozici, ale pracujeme na tom.</span><span class="sxs-lookup"><span data-stu-id="3aa25-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="3aa25-112">Pokud je šifrování na štítku zapnuté, můžete zvolit některou z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="3aa25-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="3aa25-113">Přiřazovat oprávnění nyní</span><span class="sxs-lookup"><span data-stu-id="3aa25-113">Assign permissions now</span></span>
    - <span data-ttu-id="3aa25-114">Povolit uživatelům přiřazovat oprávnění</span><span class="sxs-lookup"><span data-stu-id="3aa25-114">Let users assign permissions</span></span>


<span data-ttu-id="3aa25-115">Další informace o možných problémech najdete v článku [známé problémy s popisky citlivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="3aa25-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>