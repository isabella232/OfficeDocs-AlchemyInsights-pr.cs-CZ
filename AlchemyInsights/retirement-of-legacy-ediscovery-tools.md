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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vyřazení starších nástrojů eDiscovery

V důsledku nových a vylepšených funkcí služby eDiscovery v centru dodržování předpisů v Microsoft 365 budou v nadcházejících měsících vyřazeny následující starší nástroje a rutin.

- [Místní eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [Místní blokování](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v centru pro správu Exchange

- Rutiny PowerShellu Exchange Online, které podporují místní eDiscovery a místní blokování pro archivaci. (Tyto rutiny se společně identifikují jako rutiny *-MailboxSearch) To zahrnuje následující rutiny:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start – MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Zastavit – MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Rutina [vyhledávání – poštovní schránka](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v PowerShellu Exchange Online
- Následující operace v rozhraní API webových služeb systému Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časová osa pro odchod**:
- **1. července 2020** Už nemůžete vytvářet nová hledání a blokování, ale můžete spouštět, upravovat a odstraňovat existující vyhledávání na vlastní nebezpečí. Podpora Microsoftu nepodporují místní eDiscovery & v poli EAC.
    
- **1. října 2020** Místní eDiscovery & funkce v poli EAC se budou používat v režimu jen pro čtení, takže můžete odebrat jenom existující hledání a blokování.

**Další informace najdete v těchto tématech**:

 - [Migrace starších hledání a blokování eDiscovery do centra dodržování předpisů v Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vyřazení starších nástrojů eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Nejčastější dotazy týkající se místních eDiscovery a místních blokování pro archivaci](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



