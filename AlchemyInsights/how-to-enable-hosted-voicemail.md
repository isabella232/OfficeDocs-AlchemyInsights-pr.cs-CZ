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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="61462-102">Povolení hostované hlasové pošty</span><span class="sxs-lookup"><span data-stu-id="61462-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="61462-103">Pokud chcete povolit hlasovou schránku, musíte nastavit **HostedVoicemail** na $true.</span><span class="sxs-lookup"><span data-stu-id="61462-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="61462-104">Vlastnost **HostedVoicemail** uživatele používajícího vzdálený POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="61462-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="61462-105">Další informace o připojení k RPS najdete v tématu [Microsoft Teams PowerShell – přehled](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) Další informace o připojení k RPS.</span><span class="sxs-lookup"><span data-stu-id="61462-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="61462-106">Správce týmů by měl být přihlášen ke vzdálenému PowerShellu pro týmy.</span><span class="sxs-lookup"><span data-stu-id="61462-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="61462-107">Na příkazovém řádku PowerShell může správce Teams spustit **set-csuser user@contoso.com-HostedVoiceMail $true** , kde identifikátor URI SIP je daného uživatele.</span><span class="sxs-lookup"><span data-stu-id="61462-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="61462-108">Replikace změn zásad může trvat až 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="61462-108">Changes to policies can take up to 24 hours to replicate.</span></span>