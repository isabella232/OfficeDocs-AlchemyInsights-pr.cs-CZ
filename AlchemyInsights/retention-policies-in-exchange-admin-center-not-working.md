---
title: Zásady uchovávání informací v Exchange Admin Center nefungují
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
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074925"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zásady uchovávání informací v Exchange Admin Center

Pokud chcete, abychom spouštěli automatické kontroly nastavení uvedených níže, vyberte tlačítko Zpět <– v horní části této stránky a potom zadejte e-mailovou adresu uživatele, který má problémy se zásadami uchovávání informací.

Pokud máte problémy se zásadami uchovávání informací v Centru pro správu Exchange se na poštovní schránky nebo položky, které se do archivační poštovní schránky přesouvá, podívejte se na toto:

**Hlavní příčiny:**

- **Pomocník pro spravované** složky nezpracuje poštovní schránku uživatele. Pomocník pro spravované složky se pokusí zpracovat každou poštovní schránku ve vaší cloudové organizaci jednou za sedm dní.

  **Řešení:** Spusťte Pomocníka pro spravované složky.

- **Funkce RetentionHold** je **v** poštovní schránce povolená. Pokud je poštovní schránka umístěná na zadržovací držaně, zásady uchovávání informací v poštovní schránce se během této doby nezpracují.

  **Řešení:** Zkontrolujte stav nastavení uchovávání informací a podle potřeby aktualizujte. Podrobnosti najdete v tématu [Blokování uchovávání poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Poznámka:** Pokud je poštovní schránka menší než 10 MB, Pomocník pro spravované složky poštovní schránku automaticky nezpracuje.
 
Další informace o zásadách uchovávání informací v Centru Exchange najdete v tématu:

- [Značky uchovávání informací a zásady uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Použití zásad uchovávání informací u poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nebo [přidání nebo odebrání značek uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Jak identifikovat typ blokování umístěného v poštovní schránce](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
