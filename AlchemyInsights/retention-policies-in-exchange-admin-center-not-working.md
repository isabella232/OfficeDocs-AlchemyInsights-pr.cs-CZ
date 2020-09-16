---
title: Zásady uchovávání informací v centru pro správu Exchange nefungují
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740503"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zásady uchovávání informací v centru pro správu Exchange

Pokud chcete, abychom mohli spustit automatizované kontroly pro níže uvedené nastavení, klikněte na tlačítko zpět <--v horní části této stránky zadejte e-mailovou adresu uživatele, který má problémy se zásadami uchovávání informací.

 **Problém:** Nově vytvořené nebo aktualizované zásady uchovávání informací v centru pro správu Exchange se nevztahují na poštovní schránky ani položky, které se nepřesunou, ani se neodstraní. 
  
 **Hlavní příčiny:**
  
- Příčinou může být to, že **Pomocník pro spravovanou složku** nezpracoval poštovní schránku uživatele. Pomocník pro spravovanou složku se pokusí zpracovat každou poštovní schránku v cloudové organizaci každých 7 dní. Pokud změníte značku uchovávání informací nebo použijete jiné zásady uchovávání informací pro poštovní schránku, můžete počkat, dokud se spravovaná složka nepomůže zpracovávat, nebo spusťte rutinu Start-ManagedFolderAssistant, abyste mohli spustit konkrétní poštovní schránku. Tato rutina je užitečná pro účely testování nebo odstraňování potíží s nastavením zásad uchovávání informací nebo nastavení značek uchovávání informací. Další informace najdete v [části spuštění pomocníka pro správu složek](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Řešení:** Spuštěním následujícího příkazu spustíte Pomocníka pro správu složky pro konkrétní poštovní schránku:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Může k tomu dojít také v případě, že je na poštovní schránce **povolený** **RetentionHold** . Pokud byla poštovní schránka umístěna na RetentionHold, nebudou zásady uchovávání informací v poštovní schránce během této doby zpracovány. Další Informaton o nastavení RetentionHold najdete v tématu: [blokování zadržení poštovní schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Průzkumníku**
    
  - Zkontrolujte stav nastavení RetentionHold pro určitou poštovní schránku v [EXO PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Spuštěním následujícího příkazu **zakážete** RetentionHold v konkrétní poštovní schránce:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Spusťte znovu pomocníka Správa složek:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Poznámka:** Pokud je poštovní schránka menší než 10 MB, nebude poštovní schránka automaticky zpracovávat Pomocník pro správu složek.
 
Další informace o zásadách uchovávání informací v centru pro správu Exchange najdete v těchto tématech:
- [Značky a zásady uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Použití zásad uchovávání informací u poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Přidání nebo odebrání značek uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Jak zjistit typ blokování na poštovní schránce](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
