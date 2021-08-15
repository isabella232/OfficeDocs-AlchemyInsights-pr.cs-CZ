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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994858"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nastavení vlastnosti ClientAccessServerEnabled na hodnotu True

Pokud nemůžete otevřít zašifrovanou e-mailovou zprávu a místo toho se zobrazí **příloha rpmsg,** postupujte takto:

1. Připojení k Exchange Online PowerShellu.

> [!NOTE]
> Abyste se Exchange Online PowerShellu, musíte se přihlásit pomocí účtu globálního správce nebo Exchange správce.

   a. Otevřete Windows PowerShell a spusťte následující příkaz:`$UserCredential = Get-Credential`
b. V dialogovém **Windows PowerShell Credential Request** (Žádost o přihlašovací údaje) zadejte svůj pracovní nebo školní účet a heslo c. Klikněte na **OK**. 

2. Spuštěním následujícího příkazu vytvořte novou relaci:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Spusťte následující příkaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Příkaz `Get-IRMConfiguration` Spustit

4. Zkontrolujte **nastavení ClientAccessServerEnabled.** 

    a. Pokud **je nastavení ClientAccessServerEnabled** nastavené na **False**, spusťte následující rutinu: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Relaci powershellu vždy zavřete pomocí následujícího příkazu: `Remove-PSSession $Session`

Další informace najdete v tématu [Exchange Online PowerShellu](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

