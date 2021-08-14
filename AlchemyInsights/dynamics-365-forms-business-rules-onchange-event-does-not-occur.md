---
title: Obchodní pravidla dynamics 365 Forms – obchodní pravidlo není pro formulář vypouštěné
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
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947292"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Událost OnChange nenastane, pokud se pole změní programově.

Událost *Při změně* nedojde, pokud se pole změní programově pomocí *atributu.* [metoda setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Pokud chcete, aby se po nastavení hodnoty spustily obslužné rutiny událostí události *OnChange,* musíte v kódu použít metodu [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) *atributu formContext.data.entity.*

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
