---
title: Zásady uchovávání informací v Centru pro správu Exchange nefungují
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952221"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Zásady uchovávání informací v Centru pro správu Exchange

Pokud chcete, abychom spouštěli automatické kontroly nastavení uvedených níže, vyberte tlačítko Zpět <– v horní části této stránky a potom zadejte e-mailovou adresu uživatele, který má problémy se zásadami uchovávání informací.

Pokud máte problémy se zásadami uchovávání informací v Centru pro správu Exchange, které se neakusují u poštovních schránek nebo položek, které se do archivační poštovní schránky přesouvá, zkontrolujte toto:

**Hlavní příčiny:**

- **Pomocník pro spravované** složky nezpracuje poštovní schránku uživatele. Pomocník pro spravované složky se pokusí zpracovat každou poštovní schránku ve vaší cloudové organizaci jednou za sedm dní.

  **Řešení:** Spusťte Pomocníka pro spravované složky.

- **Funkce RetentionHold** je **v** poštovní schránce povolená. Pokud je poštovní schránka umístěná na zadržovací držaně, zásady uchovávání informací v poštovní schránce se během této doby nezpracují.

  **Řešení:** Zkontrolujte stav nastavení uchovávání informací a podle potřeby aktualizujte. Podrobnosti najdete v tématu [Blokování uchovávání poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Poznámka:** Pokud je poštovní schránka menší než 10 MB, Pomocník pro spravované složky poštovní schránku automaticky nezpracuje.
 
Další informace o zásadách uchovávání informací v Centru pro správu Exchange najdete v tématu:

- [Značky uchovávání informací a zásady uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Použití zásad uchovávání informací u poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nebo [přidání nebo odebrání značek uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Jak identifikovat typ blokování umístěného v poštovní schránce](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
