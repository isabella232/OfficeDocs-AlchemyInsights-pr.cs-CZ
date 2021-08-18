---
title: Nastavení vlastnosti ClientAccessServerEnabled na hodnotu True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320349"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nastavení vlastnosti ClientAccessServerEnabled na hodnotu True

Pokud nemůžete otevřít zašifrovanou e-mailovou zprávu a místo toho se zobrazí **příloha rpmsg,** postupujte takto:

1. Připojení k Exchange Online PowerShellu.

    **Poznámka:** Pokud se chcete Exchange Online PowerShellu, musíte se přihlásit pomocí globálního správce nebo účtu Exchange správce.

   a. Otevřete Windows PowerShell a spusťte následující příkaz:`$UserCredential = Get-Credential`
   b. V dialogovém **Windows PowerShell žádosti** o přihlašovací údaje zadejte svůj pracovní nebo školní účet a heslo, c. Klikněte na **OK**. 

2. Spuštěním následujícího příkazu vytvořte novou relaci:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Spusťte následující příkaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Příkaz `Get-IRMConfiguration` Spustit

4. Zkontrolujte **nastavení ClientAccessServerEnabled.** 

    a. Pokud **je nastavení ClientAccessServerEnabled** nastavené na **False**, spusťte následující rutinu: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tip:** Relaci powershellu vždy zavřete pomocí následujícího příkazu: `Remove-PSSession $Session`

Další informace najdete v tématu [Exchange Online PowerShellu](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

