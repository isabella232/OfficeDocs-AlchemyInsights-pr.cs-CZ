---
title: Použití Exchange Online PowerShellu k povolení DKIM pro konkrétní doménu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523636"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="643ab-102">Použití Exchange Online PowerShellu k povolení DKIM pro konkrétní doménu</span><span class="sxs-lookup"><span data-stu-id="643ab-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="643ab-103">Pokud nemůžete záznamy DNS DKIM vytvořit v Centru pro správu, zkuste použít Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="643ab-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="643ab-104">Při vytváření záznamu DNS DKIM pomocí Exchange Online PowerShellu postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="643ab-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="643ab-105">Otevřete Windows PowerShell jako správce a spusťte následující příkazy v popsaném pořadí:</span><span class="sxs-lookup"><span data-stu-id="643ab-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="643ab-106">a.</span><span class="sxs-lookup"><span data-stu-id="643ab-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="643ab-107">b.</span><span class="sxs-lookup"><span data-stu-id="643ab-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="643ab-108">c.</span><span class="sxs-lookup"><span data-stu-id="643ab-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="643ab-109">Pokud máte potíže s připojením k Exchange Online PowerShellu, podívejte se na stránku Připojení [k Exchange Online PowerShellu.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="643ab-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="643ab-110">Po připojení k Exchange Online PowerShellu spusťte následující příkaz:</span><span class="sxs-lookup"><span data-stu-id="643ab-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="643ab-111">Po úspěšném provedení příkazu spusťte následující příkaz, který ukončí relaci Exchange Online PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="643ab-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



