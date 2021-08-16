---
title: Použijte PowerShell pro zásady sdílení a vztahy organizace
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998459"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Použijte PowerShell pro zásady sdílení a vztahy organizace


Informace o relacích organizace najdete v podrobných informacích o syntaxi a parametrech pro: [Get-Federation informace](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  A  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

K vytvoření zásad sdílení použijte [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Pokud chcete [použít zásady sdílení pro poštovní schránku nebo pro uživatele](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  musíte použít kombinaci  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) a [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s nově vytvořenou zásadou. Ke  [změně, vypnutí nebo odstranění zásad sdílení](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  musíte použít  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) a [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Pokud chcete plně porozumět tomuto tématu, přečtěte si prosím:**

[Sdílení v Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)