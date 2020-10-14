---
title: Proč se aktualizace softwaru nezasazují?
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
- "9003773"
- "6717"
ms.openlocfilehash: 2e7156f994d27f46cec6dcc3c8680b55ebfe3ec2
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461753"
---
# <a name="why-software-updates-are-not-being-deployed"></a><span data-ttu-id="6b594-102">Proč se aktualizace softwaru nezasazují?</span><span class="sxs-lookup"><span data-stu-id="6b594-102">Why software updates are not being deployed?</span></span>

<span data-ttu-id="6b594-103">Pokud jste nakonfigurovali aktualizace softwaru prostřednictvím vyzvánění aktualizace Windows 10, ale aktualizace se nenasazením neprovádí, podívejte se na následující skutečnosti:</span><span class="sxs-lookup"><span data-stu-id="6b594-103">Review the following if you configured software updates through a Windows 10 update ring but the updates are not being deployed:</span></span>  

- <span data-ttu-id="6b594-104">Zvažte změnu služby Windows Servicing z  **víceletého**  typu verze na přísnější, častější typ verze</span><span class="sxs-lookup"><span data-stu-id="6b594-104">Consider changing Windows servicing from a  **Semi-Annual Channel**  release type to a stricter, more frequent release type</span></span>  
- <span data-ttu-id="6b594-105">Zkontrolujte období časově rozlišených položek pro  **aktualizaci**  a  **aktualizaci funkcí**.</span><span class="sxs-lookup"><span data-stu-id="6b594-105">Check the deferral period for  **Quality update**  and  **Feature update**.</span></span> <span data-ttu-id="6b594-106">Období časově rozlišených položek může způsobit zpoždění aktualizací po 180 dní.</span><span class="sxs-lookup"><span data-stu-id="6b594-106">The deferral period could lead to delay in updates for up 180 days.</span></span>
