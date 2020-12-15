---
title: Povolení hostované hlasové pošty
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677027"
---
# <a name="how-to-enable-hosted-voicemail"></a>Povolení hostované hlasové pošty

Pokud chcete povolit hlasovou schránku, musíte nastavit **HostedVoicemail** na $true.

Vlastnost **HostedVoicemail** uživatele používajícího vzdálený POWERSHELL (RPS).

Další informace o připojení k RPS najdete v tématu [Microsoft Teams PowerShell – přehled](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) Další informace o připojení k RPS.

1. Správce týmů by měl být přihlášen ke vzdálenému PowerShellu pro týmy.
1. Na příkazovém řádku PowerShell může správce Teams spustit **set-csuser user@contoso.com-HostedVoiceMail $true** , kde identifikátor URI SIP je daného uživatele.

> [!NOTE]
> Replikace změn zásad může trvat až 24 hodin.