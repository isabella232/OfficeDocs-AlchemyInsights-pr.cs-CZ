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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Použití Exchange Online PowerShellu k povolení DKIM pro konkrétní doménu

Pokud nemůžete záznamy DNS DKIM vytvořit v Centru pro správu, zkuste použít Exchange Online PowerShell. 

Při vytváření záznamu DNS DKIM pomocí Exchange Online PowerShellu postupujte takto:

1. Otevřete Windows PowerShell jako správce a spusťte následující příkazy v popsaném pořadí:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Pokud máte potíže s připojením k Exchange Online PowerShellu, podívejte se na stránku Připojení [k Exchange Online PowerShellu.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Po připojení k Exchange Online PowerShellu spusťte následující příkaz:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Po úspěšném provedení příkazu spusťte následující příkaz, který ukončí relaci Exchange Online PowerShellu:

    `Remove-PSSession $Session` 



