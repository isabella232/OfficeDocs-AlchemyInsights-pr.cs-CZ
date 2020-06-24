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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Použití prostředí PowerShell pro zásady sdílení a vztahy organizace


Pro vztahy organizace zkontrolujte podrobné informace o syntaxi a parametru pro: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) and [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Chcete-li vytvořit zásady sdílení, použijte [zásady Nové sdílení .](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) Chcete-li [použít zásady sdílení na poštovní schránku nebo uživatele,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) musíte použít kombinaci [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) a [get-mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s nově vytvořenými zásadami. Chcete-li [upravit, zakázat nebo odebrat zásady sdílení,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) je třeba použít [funkci Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) a [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Pro plné pochopení tohoto tématu si prosím přečtěte:**

[Sdílení v Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)