---
title: Vaše archivační poštovní schránka je téměř plná.
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046745"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Vaše archivační poštovní schránka je téměř plná.

Pokud uživatel dostane upozornění; **Archivační poštovní schránka je téměř** plná nebo potřebujete zvětšit jejich archivační poštovní schránku, tady je několik tipů:

1. Pokud má uživatel přiřazený plán Exchange Online 1, upgradujte na **licenci Exchange Online Plán 2** a zvětšete velikost z 50 GB na 100 GB.
1. Pokud už má uživatel přiřazenou některou z těchto možností: **Exchange Online Plán 2** nebo Exchange Online Plán 1 s doplňkem Exchange Online – archiv, povolte automatické rozbalení archivace pomocí následujících kroků:
 
    1. [Připojení k Exchange Online PowerShellu](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Spusťte pro uživatele následující commandlet:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Spuštěním následujícího commandletu potvrďte, že je pro uživatele povolený:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Další informace najdete v těchto informacích:

- [Povolení neomezené archivace – Nápověda pro správce – Microsoft 365 dodržování | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online limity – popisy služeb | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade na jiný plán | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

