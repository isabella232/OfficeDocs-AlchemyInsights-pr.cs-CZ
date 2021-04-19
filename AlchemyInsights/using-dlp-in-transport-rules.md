---
title: Používání DLP v pravidlech přenosu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827209"
---
# <a name="using-dlp-in-transport-rules"></a>Používání DLP v pravidlech přenosu

Pokud chcete do existujícího přenosu integrovat ochranu před únikem informací (DLP), v nastavení pravidla přenosu použijte podmínku „**Pokud zpráva obsahuje… citlivé informace**“.

**Podrobnosti viz:**

- Typy citlivých informací integrované DLP v pravidlech přenosu: [Integrace pravidel pro citlivé informace](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Pravidlo také můžete otestovat pomocí testovacího režimu, a to s testem zásad, nebo bez něj.  Než nově vytvořené pravidlo otestujete, musíte počkat 30 minut.

- Viz článek [Testování pravidel toku pošty / přenosu](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).

**Poznámka**: Pokud se pro pravidla přenosu v EAC pokoušíte zavést novou zásadu DLP, použijte místo toho [Zásady DLC v Centru zabezpečení a dodržování předpisů](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
