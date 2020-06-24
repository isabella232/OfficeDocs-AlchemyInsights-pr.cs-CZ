---
title: Použití prostředí PowerShell pro zásady sdílení a vztahy organizace
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862053"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="143f8-102">Použití prostředí PowerShell pro zásady sdílení a vztahy organizace</span><span class="sxs-lookup"><span data-stu-id="143f8-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="143f8-103">Pro vztahy organizace zkontrolujte podrobné informace o syntaxi a parametru pro: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) and [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="143f8-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="143f8-104">Chcete-li vytvořit zásady sdílení, použijte [zásady Nové sdílení .](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="143f8-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="143f8-105">Chcete-li [použít zásady sdílení na poštovní schránku nebo uživatele,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) musíte použít kombinaci [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) a [get-mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s nově vytvořenými zásadami.</span><span class="sxs-lookup"><span data-stu-id="143f8-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="143f8-106">Chcete-li [upravit, zakázat nebo odebrat zásady sdílení,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) je třeba použít [funkci Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) a [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="143f8-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="143f8-107">**Pro plné pochopení tohoto tématu si prosím přečtěte:**</span><span class="sxs-lookup"><span data-stu-id="143f8-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="143f8-108">Sdílení v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="143f8-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)