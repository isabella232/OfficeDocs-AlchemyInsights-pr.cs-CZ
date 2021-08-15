---
title: Zprávy odeslané skupině Microsoft 365 nedostávají všichni členové.
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976498"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Zprávy odeslané skupině Microsoft 365 nedostávají všichni členové.

Ujistěte se, že se všichni členové skupiny přihlásili k odběru e-mailů. Podívejte se na článek [Sledování skupiny v Outlooku](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Pokud chcete zkontrolovat stav zpráv členů, kteří se přihlásili k odběru e-mailů skupiny, spusťte následující příkaz v prostředí [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Pomocí následujícího příkazu v prostředí EXO PowerShell nakonfigurujte všechny členy skupiny tak, aby dostávali do doručené pošty e-maily odeslané skupině Microsoft 365:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Například:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`