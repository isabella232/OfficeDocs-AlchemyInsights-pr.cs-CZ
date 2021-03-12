---
title: Řešení běžných problémů s formátováním záznamů DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744885"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Řešení běžných problémů s formátováním záznamů DKIM

Většina problémů s nastavením DKIM souvisí s nesprávnými záznamy DNS.

Pokud chcete vyřešit problémy s nastavením DKIM, ověřte, jestli je záznam DKIM CNAME **(ne** záznam TXT) správně naformátovaný. Další informace najdete v článku Co je potřeba udělat pro ruční nastavení [DKIM v Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Pokud potřebujete obecně pomoct se záznamy DNS, podívejte se na stránku Vytvoření záznamů DNS u libovolného poskytovatele hostingu [DNS pro Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Po vytvoření nebo aktualizaci záznamů DNS DKIM v hostitelské službě DNS pro vaši doménu budete muset počkat, až se záznamy DNS rozšíří.
