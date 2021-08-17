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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074643"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Vyřazení starších nástrojů eDiscovery

Díky nové a vylepšené funkci eDiscovery v Centru dodržování předpisů Microsoft 365 budou v nadcházejících měsících vyřazeny následující starší nástroje eDiscovery a commandlets:

- [Služba eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [Blokování](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) na místě se nachází v centru Exchange správy.

- Rutiny Exchange Online PowerShellu, které podporují In-Place eDiscovery a In-Place Holds. (Tyto rutiny se souhrnně identifikované jako rutiny *-MailboxSearch.) Patří sem následující rutiny:

    - [Hledání v nové poštovní schránce](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Rutina [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v Exchange Online PowerShellu.
- Následující operace v rozhraní API Exchange webových služeb:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Časová osa pro odchod do důchodu**:
- **1. července 2020** Už nemůžete vytvářet nová hledání a blokování, ale existující hledání můžete spouštět, upravovat a odstraňovat na vlastní nebezpečí. Podpora Microsoftu už nepodporuje In-Place eDiscovery & Holds v EAC.
    
- **1. října 2020** In-Place eDiscovery & Funkce blokování v nástroji EAC se umístí do režimu jen pro čtení, takže můžete odebrat jenom existující hledání a blokování.

**Další informace najdete v tématu**:

 - [Migrace starších vyhledávání eDiscovery a blokování do Centrum dodržování předpisů Microsoftu 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Vyřazení starších nástrojů eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Časté otázky k In-Place eDiscovery a In-Place Blokování](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



