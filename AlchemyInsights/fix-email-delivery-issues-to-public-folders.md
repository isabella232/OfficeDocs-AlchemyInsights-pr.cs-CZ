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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366457"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Řešení problémů s doručováním e-mailů do veřejných složek s podporou pošty

Pokud externí odesílatelé nemůžou posílat zprávy do vaší poštovní složky s povoleným e-mailem a odesílatelé obdrží chybu: **nejde najít (550 5.4.1)**, ověřte, že e-mailová doména pro veřejnou složku je nakonfigurovaná jako vnitřní doména přenosu místo autoritativní domény:

1. Otevřete [Centrum pro správu Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Přejděte do **Mail flow** \> **domény přijatý**přenos, vyberte přijatou doménu a klikněte na **Upravit**.

3. Na stránce vlastnosti, která se otevře, pokud je typ domény nastaven na **autoritativní**, změňte hodnotu na **interní relé** a klikněte na **Uložit**.

Pokud externí odesílatelé obdrží chybu, **kterou nemáte oprávnění (550 5.7.13)**, spusťte následující příkaz v [PowerShellu online pro Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a zobrazte oprávnění pro anonymní uživatele ve veřejné složce:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Třeba `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Pokud chcete povolit externím uživatelům posílání e-mailů do této veřejné složky, přidejte anonymnímu uživateli oprávnění k přístupu k CreateItems. Třeba `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
