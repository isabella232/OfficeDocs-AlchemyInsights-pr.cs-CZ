---
title: Aktualizace softwaru se nesazují
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1125"
- "6700007"
ms.openlocfilehash: d9a37e4c2d977083cf2ccbf6580159f92524f936
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665243"
---
# <a name="software-updates-are-not-being-deployed"></a><span data-ttu-id="00f6d-102">Aktualizace softwaru se nesazují</span><span class="sxs-lookup"><span data-stu-id="00f6d-102">Software updates are not being deployed</span></span>

<span data-ttu-id="00f6d-103">Pokud jste nakonfigurovali aktualizace softwaru prostřednictvím vyzvánění aktualizací Windows 10, ale aktualizace se nasazují, zkuste toto:</span><span class="sxs-lookup"><span data-stu-id="00f6d-103">If you configured software updates through a Windows 10 update ring, but the updates are not being deployed, try the following:</span></span>  

- <span data-ttu-id="00f6d-104">Zvažte změnu služby Windows Servicing z  **víceletého**  typu verze na přísnější, častější typ verze.</span><span class="sxs-lookup"><span data-stu-id="00f6d-104">Consider changing Windows servicing from a  **Semi-Annual Channel**  release type to a stricter, more frequent release type.</span></span>
- <span data-ttu-id="00f6d-105">Zkontrolujte období časově rozlišených položek pro  **aktualizaci**  a  **aktualizaci funkcí**.</span><span class="sxs-lookup"><span data-stu-id="00f6d-105">Check the deferral period for  **Quality update**  and  **Feature update**.</span></span> <span data-ttu-id="00f6d-106">Období časově rozlišených položek může vést k zpoždění aktualizací až na 180 dní.</span><span class="sxs-lookup"><span data-stu-id="00f6d-106">A deferral period could lead to a delay in updates for up to 180 days.</span></span>