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
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084087"
---
# <a name="using-dlp-in-transport-rules"></a>Používání DLP v pravidlech přenosu

Pokud chcete do existujícího přenosu integrovat ochranu před únikem informací (DLP), v nastavení pravidla přenosu použijte podmínku „**Pokud zpráva obsahuje… citlivé informace**“.

**Podrobnosti viz:**

- Typy citlivých informací integrované DLP v pravidlech přenosu: [Integrace pravidel pro citlivé informace](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Pravidlo také můžete otestovat pomocí testovacího režimu, a to s testem zásad, nebo bez něj.  Než nově vytvořené pravidlo otestujete, musíte počkat 30 minut.

- Viz článek [Testování pravidel toku pošty / přenosu](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).

**Poznámka**: Pokud se pro pravidla přenosu v EAC pokoušíte zavést novou zásadu DLP, použijte místo toho [Zásady DLC v Centru zabezpečení a dodržování předpisů](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
