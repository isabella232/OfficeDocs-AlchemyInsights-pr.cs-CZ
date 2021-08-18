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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323983"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Řešení běžných problémů s formátováním záznamů DKIM

Většina problémů s nastavením DKIM souvisí s nesprávnými záznamy DNS.

Pokud chcete vyřešit problémy s nastavením DKIM, ověřte, jestli je záznam DKIM CNAME **(ne** záznam TXT) správně naformátovaný. Další informace najdete v tématu Co je potřeba udělat pro ruční nastavení [DKIM v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Pokud potřebujete obecně pomoct se záznamy DNS, podívejte se na stránku Vytvoření [záznamů DNS u libovolného](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)poskytovatele hostingu DNS pro Office 365 .

**Poznámka:** Po vytvoření nebo aktualizaci záznamů DNS DKIM v hostitelské službě DNS pro vaši doménu budete muset počkat, až se záznamy DNS rozšíří.
