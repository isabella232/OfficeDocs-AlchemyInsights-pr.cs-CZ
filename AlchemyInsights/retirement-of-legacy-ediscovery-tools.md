---
title: Vyřazení starších nástrojů eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798542"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="3d9e6-102">Vyřazení starších nástrojů eDiscovery</span><span class="sxs-lookup"><span data-stu-id="3d9e6-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="3d9e6-103">Díky nové a vylepšené funkci eDiscovery v Centru dodržování předpisů Microsoftu 365 budou následující starší nástroje eDiscovery a commandlets v nadcházejících měsících vyřazeny:</span><span class="sxs-lookup"><span data-stu-id="3d9e6-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="3d9e6-104">V Centru pro správu Exchange se nachází služba [eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [Blokování](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) na místě.</span><span class="sxs-lookup"><span data-stu-id="3d9e6-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="3d9e6-105">Rutiny PowerShellu Exchange Online, které podporují In-Place eDiscovery a In-Place blokování.</span><span class="sxs-lookup"><span data-stu-id="3d9e6-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="3d9e6-106">(Tyto rutiny se souhrnně identifikované jako rutiny \*-MailboxSearch.) Patří sem následující rutiny:</span><span class="sxs-lookup"><span data-stu-id="3d9e6-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="3d9e6-107">Hledání v nové poštovní schránce</span><span class="sxs-lookup"><span data-stu-id="3d9e6-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="3d9e6-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3d9e6-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="3d9e6-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3d9e6-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="3d9e6-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3d9e6-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="3d9e6-111">Rutina [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v Exchange Online PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="3d9e6-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="3d9e6-112">Následující operace v rozhraní API webových služeb Exchange:</span><span class="sxs-lookup"><span data-stu-id="3d9e6-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="3d9e6-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="3d9e6-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="3d9e6-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3d9e6-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="3d9e6-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3d9e6-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="3d9e6-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="3d9e6-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="3d9e6-117">**Časová osa pro odchod do důchodu**:</span><span class="sxs-lookup"><span data-stu-id="3d9e6-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="3d9e6-118">**1. července 2020** Už nemůžete vytvářet nová hledání a blokování, ale existující hledání můžete spouštět, upravovat a odstraňovat na vlastní nebezpečí.</span><span class="sxs-lookup"><span data-stu-id="3d9e6-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="3d9e6-119">Podpora Microsoftu už nepodporuje In-Place eDiscovery & Holds v EAC.</span><span class="sxs-lookup"><span data-stu-id="3d9e6-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="3d9e6-120">**1. října 2020** In-Place eDiscovery & Funkce blokování v nástroji EAC se umístí do režimu jen pro čtení, takže můžete odebrat jenom existující hledání a blokování.</span><span class="sxs-lookup"><span data-stu-id="3d9e6-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="3d9e6-121">**Další informace najdete v tématu**:</span><span class="sxs-lookup"><span data-stu-id="3d9e6-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="3d9e6-122">Migrace starších vyhledávání a blokování eDiscovery do Centra dodržování předpisů Microsoftu 365</span><span class="sxs-lookup"><span data-stu-id="3d9e6-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="3d9e6-123">Vyřazení starších nástrojů eDiscovery</span><span class="sxs-lookup"><span data-stu-id="3d9e6-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="3d9e6-124">Časté otázky k In-Place eDiscovery a In-Place Blokování</span><span class="sxs-lookup"><span data-stu-id="3d9e6-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



