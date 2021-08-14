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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930054"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Řešení běžných problémů s formátováním záznamů DKIM

Většina problémů s nastavením DKIM souvisí s nesprávnými záznamy DNS.

Pokud chcete vyřešit problémy s nastavením DKIM, ověřte, jestli je záznam DKIM CNAME **(ne** záznam TXT) správně naformátovaný. Další informace najdete v tématu Co je potřeba udělat pro ruční nastavení [DKIM v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Pokud potřebujete pomoct se záznamy DNS obecně, podívejte se na stránku Vytvoření [záznamů DNS u libovolného](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)poskytovatele hostingu DNS pro Office 365 .

> [!NOTE]
> Po vytvoření nebo aktualizaci záznamů DNS DKIM v hostitelské službě DNS pro vaši doménu budete muset počkat, až se záznamy DNS rozšíří.
