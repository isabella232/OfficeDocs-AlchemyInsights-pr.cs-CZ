---
title: Business Rules aplikace Dynamics 365 – firemní pravidlo pro formulář se neaktivují
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711484"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>K události při změně nedojde při programové změně pole

K události při *změně* nedojde, pokud se pole pomocí atributu změní programově *.* Metoda [NastavitHodnotu](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Pokud chcete, aby se obslužné rutiny událostí při události při *změně* spustily po nastavení hodnoty, musíte v kódu použít metodu [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) *formContext. data. entity* .

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
