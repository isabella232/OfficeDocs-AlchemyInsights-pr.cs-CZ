---
title: Jak povolit hostovanou hlasovou poštu
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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318641"
---
# <a name="how-to-enable-hosted-voicemail"></a>Jak povolit hostovanou hlasovou poštu

Pokud chcete povolit hlasovou poštu, musí být **HostedVoicemail** nastavený na $true.

Vlastnost **HostedVoicemail** pro uživatele pomocí vzdáleného PowerShellu (RPS).

Další informace o připojení k RPS najdete v článku [Microsoft Teams PowerShellu –](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) přehled, který obsahuje další informace o připojení k RPS.

1. Správce Teams by měl být přihlášený ke vzdálenému PowerShellu pro Teams.
1. V powershellové výzvě může správce Teams **spustit set-csuser user@contoso.com -HostedVoiceMail $true** kde sip uri je ovládacího prvku uživatele.

**Poznámka:** Replikace změn zásad může trvat až 24 hodin.