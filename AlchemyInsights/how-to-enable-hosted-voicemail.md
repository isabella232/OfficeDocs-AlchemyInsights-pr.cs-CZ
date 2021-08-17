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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055547"
---
# <a name="how-to-enable-hosted-voicemail"></a>Jak povolit hostovanou hlasovou poštu

Pokud chcete povolit hlasovou poštu, musí být **HostedVoicemail** nastavený na $true.

Vlastnost **HostedVoicemail** pro uživatele pomocí vzdáleného PowerShellu (RPS).

Další informace o připojení k RPS najdete v článku [Microsoft Teams PowerShellu –](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) přehled, který obsahuje další informace o připojení k RPS.

1. Správce Teams by měl být přihlášený ke vzdálenému PowerShellu pro Teams.
1. V powershellové výzvě může správce Teams **spustit set-csuser user@contoso.com -HostedVoiceMail $true,** kde je identifikátor uri sip ovládacího prvku uživatele.

> [!NOTE]
> Replikace změn zásad může trvat až 24 hodin.