---
title: Zásady uchovávání informací v Centru pro správu Exchange nefungují
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522800"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zásady uchovávání informací v Centru pro správu Exchange

Pokud chcete, abychom spouštěli automatické kontroly níže uvedených nastavení, vyberte v horní části této stránky tlačítko Zpět < a zadejte e-mailovou adresu uživatele, který má problémy se zásadami uchovávání informací.

 **Problém:** Nově vytvořené nebo aktualizované zásady uchovávání informací v Centru pro správu Exchange se nevztahují na poštovní schránky nebo položky nejsou přesunuty do poštovní schránky archivu nebo odstraněny. 
  
 **Příčiny:**
  
- Důvodem může být, že **Pomocník pro spravované složky** nezpracoval poštovní schránku uživatele. Pomocník pro spravované složky se pokusí zpracovat každou poštovní schránku v organizaci na principu shluků jednou za sedm dní. Pokud změníte značku uchovávání informací nebo použijete jinou zásadu uchovávání informací pro poštovní schránku, můžete počkat, dokud pomoc s spravované složky zpracuje poštovní schránku, nebo můžete spustit rutinu Start-ManagedFolderAssistant a spustit Pomocníka pro spravované složky ke zpracování konkrétní poštovní schránky. Spuštění této rutiny je užitečné pro testování nebo řešení potíží se zásadami uchovávání informací nebo nastavením značky uchovávání informací. Další informace naleznete na stránce [Spuštění Pomocníka pro spravované složky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Řešení:** Spuštěním následujícího příkazu spusťte Pomocníka pro spravované složky pro určitou poštovní schránku:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- K tomu může dojít také v **případě, že retentionhold** byla **povolena** v poštovní schránce. Pokud poštovní schránka byla umístěna na RetentionHold, zásady uchovávání informací v poštovní schránce nebudou zpracovány během této doby. Další informace o nastavení retentionhold najdete v tématu: [Blokování uchovávání poštovní schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Řešení:**
    
  - Zkontrolujte stav nastavení RetentionHold na konkrétní poštovní schránce v [prostředí EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Spuštěním následujícího příkazu **zakázat** RetentionHold na konkrétní poštovní schránky:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nyní znovu spusťte Pomocníka pro spravované složky:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Poznámka:** Pokud je poštovní schránka menší než 10 MB, Pomocník pro spravované složky poštovní schránku automaticky nezpracuje.
 
Další informace o zásadách uchovávání informací v Centru pro správu Exchange najdete v následujících tématech:
- [Značky uchovávání informací a zásady uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Použití zásad uchovávání informací u poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Přidání nebo odebrání značek uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Jak identifikovat typ blokování umístěného v poštovní schránce](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
