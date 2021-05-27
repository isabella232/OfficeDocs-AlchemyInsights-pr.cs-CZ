---
title: Inventář softwaru chybí nebo je nepřesný
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676141"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="cf088-102">Inventář softwaru chybí nebo je nepřesný</span><span class="sxs-lookup"><span data-stu-id="cf088-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="cf088-103">Inventář softwaru v Threat and Vulnerability Management (TVM) je seznam známých softwaru ve vaší organizaci s oficiálními výčty společných platforem (CPE).</span><span class="sxs-lookup"><span data-stu-id="cf088-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="cf088-104">Softwarové produkty bez oficiální cpe nemají publikované chyby zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="cf088-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="cf088-105">Inventář obsahuje také podrobnosti, jako je jméno dodavatele, počet nedostatků, hrozby a počet exponovaných zařízení.</span><span class="sxs-lookup"><span data-stu-id="cf088-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="cf088-106">Změny softwaru na zařízeních se obvykle projeví na portálech zabezpečení do dvou hodin.</span><span class="sxs-lookup"><span data-stu-id="cf088-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="cf088-107">Někdy to ale může trvat déle.</span><span class="sxs-lookup"><span data-stu-id="cf088-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="cf088-108">Momentálně není žádný způsob, jak vynutit synchronizaci. jedná se o průběžné průběžné hodnocení.</span><span class="sxs-lookup"><span data-stu-id="cf088-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="cf088-109">Pokud jste provedli změnu softwaru a změna se přesně neprojeví v TVM po 5 hodinách, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="cf088-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="cf088-110">Informace o tom, jak byl software zjištěn, si můžete zjistit v části s důkazy softwaru.</span><span class="sxs-lookup"><span data-stu-id="cf088-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="cf088-111">Ujistěte se, že je software podporovaný.</span><span class="sxs-lookup"><span data-stu-id="cf088-111">Make sure that the software is supported.</span></span> <span data-ttu-id="cf088-112">Software může být viditelný jenom na úrovni zařízení, i když ho v současné době Threat and Vulnerability Management.</span><span class="sxs-lookup"><span data-stu-id="cf088-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="cf088-113">K dispozici jsou ale jenom omezená data.</span><span class="sxs-lookup"><span data-stu-id="cf088-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="cf088-114">Postup hlášení nepřesnosti z portálu najdete v článku [Nahlášení nepřesnosti](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="cf088-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="cf088-115">**Poznámka:** Hlášení nepřesnosti z portálu MDE je jednosměnný kanál k technice.</span><span class="sxs-lookup"><span data-stu-id="cf088-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="cf088-116">Pokud je problém naléhavý, otevřete lístek podpory.</span><span class="sxs-lookup"><span data-stu-id="cf088-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="cf088-117">Další informace najdete v tématu [Inventář softwaru – Threat and Vulnerability Management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="cf088-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>