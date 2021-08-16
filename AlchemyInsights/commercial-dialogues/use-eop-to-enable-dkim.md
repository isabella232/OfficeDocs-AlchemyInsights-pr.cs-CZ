---
title: Použití Exchange Online PowerShellu k povolení DKIM pro určitou doménu
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070286"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Použití Exchange Online PowerShellu k povolení DKIM pro určitou doménu

Pokud nemůžete vytvořit záznamy DNS DKIM v Centru pro správu, zkuste použít Exchange Online PowerShellu. 

Pokud chcete vytvořit záznam DNS DKIM Exchange Online PowerShellu, postupujte takto:

1. Otevřete Windows PowerShell jako správce a v popsaném pořadí spusťte následující příkazy:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Pokud máte potíže s připojením k Exchange Online PowerShellu, podívejte [se Připojení na Exchange Online PowerShellu.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Až budete připojení k Exchange Online PowerShellu, spusťte následující příkaz:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Po úspěšném spuštění výše uvedeného příkazu spusťte následující příkaz, který ukončí relaci Exchange Online PowerShellu:

    `Remove-PSSession $Session` 



