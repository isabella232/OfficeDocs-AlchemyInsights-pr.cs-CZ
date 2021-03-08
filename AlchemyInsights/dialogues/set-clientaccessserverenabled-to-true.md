---
title: Nastavení clientAccessServerEnabled na Hodnotu True
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523833"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nastavení clientAccessServerEnabled na Hodnotu True

Pokud nemůžete zašifrovanou e-mailovou zprávu otevřít a místo toho uvidíte přílohu zprávy **o** otevření, postupujte takto:

1. Připojte se k Exchange Online PowerShellu.

> [!NOTE]
> Pokud se chcete připojit k Exchange Online PowerShellu, musíte se přihlásit pomocí účtu globálního správce nebo správce Exchange.

   a. Otevřete Windows PowerShell a spusťte následující příkaz: `$UserCredential = Get-Credential`
b. V dialogovém **okně Windows PowerShell Credential Request** (Žádost o pověření windows PowerShellu) zadejte svůj pracovní nebo školní účet a heslo, c. Klikněte na tlačítko **OK**. 

2. Spuštěním následujícího příkazu vytvořte novou relaci:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Spusťte tento příkaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Příkaz `Get-IRMConfiguration` Spustit

4. Zkontrolujte nastavení **ClientAccessServerEnabled.** 

    a. Pokud **je nastavení ClientAccessServerEnabled** nastavené na **False,** spusťte následující rutinu: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Relaci PowerShellu vždycky zavřete pomocí následujícího příkazu: `Remove-PSSession $Session`

Další informace najdete v článku [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

