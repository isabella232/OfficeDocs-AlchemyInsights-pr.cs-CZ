---
title: Testování kompatibility aplikací
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692721"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="782d5-102">Testování kompatibility aplikací</span><span class="sxs-lookup"><span data-stu-id="782d5-102">Do app compatibility testing</span></span>

<span data-ttu-id="782d5-103">Kompatibilita aplikací pro Microsoft Edge je mimořádně vysoká.</span><span class="sxs-lookup"><span data-stu-id="782d5-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="782d5-104">Je skutečně tak vysoká, že Microsoft nabízí následující sliby kompatibility:</span><span class="sxs-lookup"><span data-stu-id="782d5-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="782d5-105">Pokud funguje v Microsoft Edge 45 a starších verzích, bude fungovat v Microsoft Edge 77 a novějších verzích.</span><span class="sxs-lookup"><span data-stu-id="782d5-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="782d5-106">Pokud funguje v Internet Exploreru, bude fungovat v prohlížeči Microsoft Edge v režimu Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="782d5-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="782d5-107">Pokud funguje v Google Chromu, bude fungovat v Microsoft Prohlížeči Edge.</span><span class="sxs-lookup"><span data-stu-id="782d5-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="782d5-108">Pokud máte aplikaci, ve které tento příslib nesplňujeme, stojíme za příslibem, že ji opravíme pomocí [aplikace Microsoft App Assure.](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)</span><span class="sxs-lookup"><span data-stu-id="782d5-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="782d5-109">I přes tento příslib si víme, že mnoho organizací musí ověřit některé aplikace z důvodu dodržování předpisů nebo řízení rizik.</span><span class="sxs-lookup"><span data-stu-id="782d5-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="782d5-110">I když očekáváme, že to bude velmi jednoduché, je důležité, abyste byli při testování aplikací organizovaní a pečliví.</span><span class="sxs-lookup"><span data-stu-id="782d5-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="782d5-111">Testování kompatibility aplikací můžete provést dvěma způsoby:</span><span class="sxs-lookup"><span data-stu-id="782d5-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="782d5-112">**Testování v laboratoři:** Aplikace se testují v prostředí s velmi řízeným řízením s konkrétními konfiguracemi.</span><span class="sxs-lookup"><span data-stu-id="782d5-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="782d5-113">**Pilotní testování:** Aplikace jsou testovány omezeným počtem uživatelů ve svém každodenním pracovním prostředí pomocí vlastních zařízení.</span><span class="sxs-lookup"><span data-stu-id="782d5-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="782d5-114">Zvolte metodu, která je pro každou aplikaci nejvhodnější, a před spuštěním v celé organizaci proveďte testování.</span><span class="sxs-lookup"><span data-stu-id="782d5-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="782d5-115">Až zajistíte, že jsou vaše aplikace kompatibilní, můžete Microsoft Edge nasadit do pilotní skupiny.</span><span class="sxs-lookup"><span data-stu-id="782d5-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
