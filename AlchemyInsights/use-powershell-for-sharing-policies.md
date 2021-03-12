---
title: Použijte PowerShell pro zásady sdílení a vztahy organizace
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
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709459"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="64dc9-102">Použijte PowerShell pro zásady sdílení a vztahy organizace</span><span class="sxs-lookup"><span data-stu-id="64dc9-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="64dc9-103">Informace o relacích organizace najdete v podrobných informacích o syntaxi a parametrech pro: [Get-Federation informace](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  A  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="64dc9-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="64dc9-104">K vytvoření zásad sdílení použijte [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="64dc9-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="64dc9-105">Pokud chcete [použít zásady sdílení pro poštovní schránku nebo pro uživatele](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  musíte použít kombinaci  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) a [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s nově vytvořenou zásadou.</span><span class="sxs-lookup"><span data-stu-id="64dc9-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="64dc9-106">Ke  [změně, vypnutí nebo odstranění zásad sdílení](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  musíte použít  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) a [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="64dc9-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="64dc9-107">**Pokud chcete plně porozumět tomuto tématu, přečtěte si prosím:**</span><span class="sxs-lookup"><span data-stu-id="64dc9-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="64dc9-108">Sdílení v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="64dc9-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)