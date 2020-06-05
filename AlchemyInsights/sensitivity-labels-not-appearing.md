---
title: Popisky citlivosti se nezobrazují
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581008"
---
# <a name="sensitivity-labels-not-appearing"></a>Popisky citlivosti se nezobrazují

Popisky citlivosti umožňují klasifikovat a chránit citlivý obsah. Mohou být vytvořeny v Centru dodržování předpisů Microsoft 365, Microsoft 365 Security Center nebo Microsoft 365 Security & Compliance Center v rámci popisků klasifikace > citlivosti. Další informace o této funkci naleznete v [tématu Přehled popisků citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Pokud jste nakonfigurovali štítky citlivosti, ale nezobrazují se v aplikacích Microsoft 365, zkontrolujte následující:

- Zkontrolujte, zda byl popisek [citlivosti publikován](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) uživatelům a požadovaným skupinám.

- Zkontrolujte, zda uživatel používá aplikaci, která podporuje popisky citlivosti – [viz popisky citlivosti v dokumentu](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Pokud [migrujete popisky Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), mějte na paměti zde [uvedené](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)důležité informace .

- Podpora ochrany před únikem informací (DLP): V současné době lze jako podmínku v zásadách ochrany před únikem informací použít jako podmínku pouze popisky uchovávání informací.  Podpora popisků citlivosti v zásadách ochrany před únikem dat ještě není k dispozici, ale pracujeme na ní.

- Pokud je šifrování povoleno na štítku citlivosti, můžete zvolit:
    - Přiřazovat oprávnění
    - Povolit uživatelům přiřazovat oprávnění


Další informace o možných problémech naleznete v [tématu Známé problémy s popisky citlivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).