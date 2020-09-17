---
title: Kód chyby 550 5.7.501 přístup odepřen, zjištěn spam nevyžádaný
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784048"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 přístup odepřen, zjištěn spam nevyžádaný

Tato zpráva se obvykle zobrazí, když uživatelé odesílají e-mailové zprávy z IP adres pomocí počáteční domény *onmicrosoft.com* přiřazené novým klientům v Microsoft 365. Nejjednodušším způsobem, jak tento problém vyřešit:

1. [Přidejte doménu ke svému tenantovi](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Změňte primární e-mailovou adresu uživatelů](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) na nově přidanou doménu.
