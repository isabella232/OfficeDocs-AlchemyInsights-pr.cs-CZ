---
title: Povolení funkce DKIM pro konkrétní doménu pomocí Exchange Online PowerShellu
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744650"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Povolení funkce DKIM pro konkrétní doménu pomocí Exchange Online PowerShellu

Pokud nemůžete vytvořit záznamy DNS DKIM v Centru pro správu, zkuste použít Exchange Online PowerShell. 

Pokud chcete vytvořit záznam DNS DKIM pomocí Exchange Online PowerShellu, postupujte takto:

1. Otevřete Windows PowerShell jako správce a v popsaném pořadí spusťte následující příkazy:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Pokud máte potíže s připojením k Exchange Online PowerShellu, podívejte se na stránku [Připojení k Exchange Online PowerShellu.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Až budete připojení k Exchange Online PowerShellu, spusťte následující příkaz:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Po úspěšném spuštění výše uvedeného příkazu ukončete relaci Exchange Online PowerShellu spuštěním následujícího příkazu:

    `Remove-PSSession $Session` 



