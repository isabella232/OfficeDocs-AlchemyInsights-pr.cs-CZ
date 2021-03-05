---
title: Problém s atributem a filtrem rozsahu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481099"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="f3529-102">Problém s atributem a filtrem rozsahu</span><span class="sxs-lookup"><span data-stu-id="f3529-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="f3529-103">**Problém s konfliktním hodnotami UPN**</span><span class="sxs-lookup"><span data-stu-id="f3529-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="f3529-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.**</span><span class="sxs-lookup"><span data-stu-id="f3529-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="f3529-105">Operace se nezdařila, protože hodnota celého ovládacího název uživatele (UPN) zadaná pro přidání nebo úpravy není jedinečná v celé doménové struktuře.</span><span class="sxs-lookup"><span data-stu-id="f3529-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="f3529-106">Podrobnosti chyby: **CONSTRAINT_ATT_TYPE - userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="f3529-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="f3529-107">Hodnota **userPrincipalName,** která se snaží nastavit konektor Workday při vytváření uživatelského účtu služby AD, už v cílové doméně služby AD existuje.</span><span class="sxs-lookup"><span data-stu-id="f3529-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="f3529-108">Znamená to, že některý (1) uživatel už existuje a odpovídající kontrola ID se pro uživatele nezdařila, nebo (2) pravidlo generování upn vygeneroval konfliktní hodnotu.</span><span class="sxs-lookup"><span data-stu-id="f3529-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="f3529-109">Tady jsou navrhované kroky řešení:</span><span class="sxs-lookup"><span data-stu-id="f3529-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="f3529-110">Pokud už uživatel existuje a odpovídající kontrola ID se nepovedlo propojit účet Workday s účtem Active Directory, zkontrolujte, jestli odpovídající atribut ID (obvykle ID **zaměstnance)** v workday i AD obsahuje přesnou shodu.</span><span class="sxs-lookup"><span data-stu-id="f3529-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="f3529-111">Pokud se neshodují, je to problém s daty, který je potřeba opravit.</span><span class="sxs-lookup"><span data-stu-id="f3529-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="f3529-112">Pokud je třeba ID zaměstnance v pracovní den 001052 a v ad je 1052, modul zřizování tyto dva účty nepropojí a pokusí se vytvořit uživatele, který už existuje.</span><span class="sxs-lookup"><span data-stu-id="f3529-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="f3529-113">Řešením v tomto případě je změnit hodnotu **ID** Zaměstnance v ad tak, aby zahrnovala počáteční nuly na 001052.</span><span class="sxs-lookup"><span data-stu-id="f3529-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="f3529-114">Pokud výraz, který generuje hlavní název uživatele, negeneruje jedinečnou hodnotu, zvažte možnost použít funkci **SelectUniqueValue** deplikace, která pokaždé vygeneruje jedinečnou hodnotu.</span><span class="sxs-lookup"><span data-stu-id="f3529-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="f3529-115">**U uživatelského účtu služby AD Workday se nenastaví hodnota atributu správce pro uživatelský účet služby AD.**</span><span class="sxs-lookup"><span data-stu-id="f3529-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="f3529-116">Úloha Workday to AD User Provisioning nenastavuje hodnotu **atributu správce** pro uživatelské účty služby AD.</span><span class="sxs-lookup"><span data-stu-id="f3529-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="f3529-117">Existují dva možné scénáře, kdy se toto chování zobrazí:</span><span class="sxs-lookup"><span data-stu-id="f3529-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="f3529-118">Vedoucího v pracovní dny nelze rozpoznat na odpovídající uživatelský účet služby AD, protože nad rámec nemá.</span><span class="sxs-lookup"><span data-stu-id="f3529-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="f3529-119">Ve **scénáři s víc** doménami ad není vedoucí v pracovní dny ve stejné doméně jako uživatel.</span><span class="sxs-lookup"><span data-stu-id="f3529-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="f3529-120">Zkuste tento problém vyřešit pomocí následujících kroků:</span><span class="sxs-lookup"><span data-stu-id="f3529-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="f3529-121">Pokud jste definovali filtry rozsahu, nejdřív zkontrolujte, jestli vedoucí má obor a jestli splňuje klauzuli pro vymezení rozsahu.</span><span class="sxs-lookup"><span data-stu-id="f3529-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="f3529-122">Pokud manažer filtr oboru nesplňuje, změňte filtr tak, aby vedoucí byl také v rozsahu operace zřizování.</span><span class="sxs-lookup"><span data-stu-id="f3529-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="f3529-123">Pokud máte víc domén AD, má spojnice známé omezení, že se neřeší odkazy na správce křížových domén.</span><span class="sxs-lookup"><span data-stu-id="f3529-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="f3529-124">Další podrobnosti o konfiguraci pracovního dne pro automatické zřizování najdete v kurzu: Konfigurace [funkce Workday pro automatické zřizování uživatelů.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="f3529-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













