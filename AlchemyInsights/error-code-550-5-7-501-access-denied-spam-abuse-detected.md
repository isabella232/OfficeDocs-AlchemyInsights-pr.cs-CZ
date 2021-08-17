---
title: Kód chyby 550 5.7.501 Access denied, spam abuse detected
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
ms.openlocfilehash: a3eebe4e9d69e100a750e74a6d34ec67dc0566df5dd6eb59809adb07ed8a682f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044261"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Access denied, spam abuse detected

K této zprávě obvykle dochází, když uživatelé odesílali e-mailové zprávy z IP adres pomocí počáteční domény *.onmicrosoft.com,* která je přiřazená novým tenantům v Microsoft 365. Nejjednodušší způsob, jak tento problém vyřešit, je:

1. [Přidejte doménu do tenanta](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Změňte primární e-mailovou adresu uživatelů](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) na novou vlastní doménu, kterou jste právě přidali.
