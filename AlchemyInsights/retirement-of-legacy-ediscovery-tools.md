---
title: Vyřazení starších nástrojů eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727776"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="f193a-102">Vyřazení starších nástrojů eDiscovery</span><span class="sxs-lookup"><span data-stu-id="f193a-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="f193a-103">V důsledku nových a vylepšených funkcí služby eDiscovery v centru dodržování předpisů v Microsoft 365 budou v nadcházejících měsících vyřazeny následující starší nástroje a rutin.</span><span class="sxs-lookup"><span data-stu-id="f193a-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="f193a-104">[Místní eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [Místní blokování](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v centru pro správu Exchange</span><span class="sxs-lookup"><span data-stu-id="f193a-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="f193a-105">Rutiny PowerShellu Exchange Online, které podporují místní eDiscovery a místní blokování pro archivaci.</span><span class="sxs-lookup"><span data-stu-id="f193a-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="f193a-106">(Tyto rutiny se společně identifikují jako rutiny \*-MailboxSearch) To zahrnuje následující rutiny:</span><span class="sxs-lookup"><span data-stu-id="f193a-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="f193a-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f193a-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="f193a-108">Start – MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f193a-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="f193a-109">Zastavit – MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f193a-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="f193a-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f193a-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="f193a-111">Rutina [vyhledávání – poštovní schránka](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v PowerShellu Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f193a-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="f193a-112">Následující operace v rozhraní API webových služeb systému Exchange:</span><span class="sxs-lookup"><span data-stu-id="f193a-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="f193a-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="f193a-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="f193a-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f193a-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="f193a-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f193a-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="f193a-116">Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="f193a-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="f193a-117">**Časová osa pro odchod**:</span><span class="sxs-lookup"><span data-stu-id="f193a-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="f193a-118">**1. července 2020** Už nemůžete vytvářet nová hledání a blokování, ale můžete spouštět, upravovat a odstraňovat existující vyhledávání na vlastní nebezpečí.</span><span class="sxs-lookup"><span data-stu-id="f193a-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="f193a-119">Podpora Microsoftu nepodporují místní eDiscovery & v poli EAC.</span><span class="sxs-lookup"><span data-stu-id="f193a-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="f193a-120">**1. října 2020** Místní eDiscovery & funkce v poli EAC se budou používat v režimu jen pro čtení, takže můžete odebrat jenom existující hledání a blokování.</span><span class="sxs-lookup"><span data-stu-id="f193a-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="f193a-121">**Další informace najdete v těchto tématech**:</span><span class="sxs-lookup"><span data-stu-id="f193a-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="f193a-122">Migrace starších hledání a blokování eDiscovery do centra dodržování předpisů v Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f193a-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="f193a-123">Vyřazení starších nástrojů eDiscovery</span><span class="sxs-lookup"><span data-stu-id="f193a-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="f193a-124">Nejčastější dotazy týkající se místních eDiscovery a místních blokování pro archivaci</span><span class="sxs-lookup"><span data-stu-id="f193a-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



