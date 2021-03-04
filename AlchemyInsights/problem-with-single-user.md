---
title: Problém s jedním uživatelem
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429467"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="69d9e-102">Problém s jedním uživatelem</span><span class="sxs-lookup"><span data-stu-id="69d9e-102">Problem with single user</span></span>

- <span data-ttu-id="69d9e-103">Uživatel možná nebyl zřízen, protože služba ještě nemá možnost uživatele vyhodnotit.</span><span class="sxs-lookup"><span data-stu-id="69d9e-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="69d9e-104">Prohlédněte si pokyny, jak dlouho bude zřizování a indikátor průběhu na stránce pro konfiguraci zřizování trvat.</span><span class="sxs-lookup"><span data-stu-id="69d9e-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="69d9e-105">Pokud se stabilní stav zadaný v části s dalšími podrobnostmi nachází před datem, kdy byl uživatel vytvořen, aktualizován nebo odstraněn, znamená to, že jsme uživatele ještě nevyhodnocili.</span><span class="sxs-lookup"><span data-stu-id="69d9e-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="69d9e-106">V tomto scénáři je nejlepší počkat, až se dokončí zřizovací služba.</span><span class="sxs-lookup"><span data-stu-id="69d9e-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="69d9e-107">Mějte na paměti, že naše služba je o změnách uživatele ve zdrojovém systému (cloudové personální oddělení).</span><span class="sxs-lookup"><span data-stu-id="69d9e-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="69d9e-108">Aby azure AD detekuje změnu a přetékal do Active Directory, musí být ve zdrojovém systému platná změna.</span><span class="sxs-lookup"><span data-stu-id="69d9e-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="69d9e-109">Služba zřizování vyhodnocela uživatele a určila, že nemá být zřízena:</span><span class="sxs-lookup"><span data-stu-id="69d9e-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="69d9e-110">Pokud jste nastavili filtr rozsahu založený na atributu, přesvědčte se, zda uživatel splňuje zadaná kritéria.</span><span class="sxs-lookup"><span data-stu-id="69d9e-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="69d9e-111">Pokud už uživatelé existují v cílovém systému a stav uživatele ve zdrojové a cílové shodě, nebudeme už nic dalšího provést.</span><span class="sxs-lookup"><span data-stu-id="69d9e-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="69d9e-112">Služba zřizování se pokusila zřídit uživatele, ale selhala.</span><span class="sxs-lookup"><span data-stu-id="69d9e-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="69d9e-113">U těchto scénářů si prohlédněte kartu řešení potíží a doporučení v protokolech zřizování:</span><span class="sxs-lookup"><span data-stu-id="69d9e-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="69d9e-114">Atribut, který uživatel požaduje, může chybět v místní službě Active Directory nebo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69d9e-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="69d9e-115">Například pravidla generace userPrincipalName nebo sAMAccountName negenerují správnou hodnotu.</span><span class="sxs-lookup"><span data-stu-id="69d9e-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="69d9e-116">Odpovídající atribut (obvykle employeeId) se nevyřešuje jedinečnému uživateli v místní službě Active Directory nebo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69d9e-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="69d9e-117">Například dva uživatelé se stejným id zaměstnance ve službě AD a služba vrátí kód chyby, který označuje duplicitní cílové položky pro stejnou zdrojovou položku.</span><span class="sxs-lookup"><span data-stu-id="69d9e-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="69d9e-118">Pokud chcete zkontrolovat protokoly pro jednotlivé uživatele a skupiny, podívejte se na téma Kontrola protokolů zřizování pro problém [s konkrétním uživatelem.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="69d9e-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
