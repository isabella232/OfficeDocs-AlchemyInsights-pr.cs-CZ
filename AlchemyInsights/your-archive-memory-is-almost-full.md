---
title: Vaše archivní poštovní schránka je skoro plná
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974212"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Vaše archivní poštovní schránka je skoro plná

Pokud uživatel obdrží upozornění; **Vaše archivní poštovní schránka je skoro plná** nebo potřebujete zvětšit velikost archivované poštovní schránky:

1. Pokud je uživateli přiřazený online plán 1, upgradujte na licenci **Exchange Online Plan 2** , abyste zvýšili velikost z 50 GB na 100GB.
1. Pokud je uživatel už přiřazený: **Exchange Online (plán 2** ) nebo Exchange Online (plán 1) s doplňkem Exchange Online pro archivaci, použijte k povolení automatického rozbalování archivování následující postup:
 
    1. [Připojení k PowerShellu služby Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Pro uživatele spusťte následující unifiedgroup:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Potvrďte povolení pro uživatele spuštěním následujícího unifiedgroup:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Další informace najdete v těchto tématech:

- [ Povolit neomezené archivace – Nápověda pro správce – dodržování předpisů Microsoft 365 | Dokumenty Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limity pro Exchange Online – popisy služeb | Dokumenty Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade na jiný firemní plán | Dokumenty Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

