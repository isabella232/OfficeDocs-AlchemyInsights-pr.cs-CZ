---
title: Řešení problémů s doručováním e-mailů do veřejných složek s podporou pošty
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068805"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Řešení problémů s doručováním e-mailů do veřejných složek s podporou pošty

Pokud externí odesílatelé nemohli posílat zprávy do veřejných složek s podporou pošty a odesílatelům se zobrazí chybová zpráva: Nelze najít **(550 5.4.1),** ověřte, jestli je e-mailová doména veřejné složky nakonfigurovaná jako doména interního přenosu místo autoritativní domény:

1. Otevřete Centrum [Exchange pro správu (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Přejděte na **Mail flow** Accepted \> domains (Přijaté **domény** toku pošty), vyberte přijatou doménu a klikněte na **Upravit.**

3. Na stránce vlastností, která se otevře, pokud je typ domény nastavený na Autoritativní **,** změňte hodnotu na **Interní přenos** a klikněte na **Uložit.**

Pokud se externím odesílatelům zobrazí chybová zpráva, že nemáte oprávnění **(550 5.7.13),** spusťte v [Exchange Online PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) následující příkaz, který zobrazí oprávnění anonymních uživatelů ve veřejné složce:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Například . `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`

Pokud chcete externím uživatelům povolit posílání e-mailů do této veřejné složky, přidejte přístupové právo CreateItems k anonymnímu uživateli. Například . `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`
