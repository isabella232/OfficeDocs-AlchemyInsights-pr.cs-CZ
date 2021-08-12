---
title: Popisky citlivosti se nezobrazují
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061425"
---
# <a name="sensitivity-labels-not-appearing"></a>Popisky citlivosti se nezobrazují

Popisky citlivosti umožňují klasifikovat a chránit váš citlivý obsah. Můžete je vytvořit v centru Centrum dodržování předpisů Microsoftu 365, Microsoft 365 zabezpečení nebo v centru Microsoft 365 zabezpečení & v části Klasifikační > citlivosti. Další informace o této funkci najdete v tématu [Přehled popisků citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Pokud jste nakonfigurovali popisky citlivosti, ale nezobrazují se v Microsoft 365 aplikacích, zkontrolujte následující:

- Ověřte, že popisek citlivosti byl [publikovaný](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) pro uživatele a skupiny, které chcete.

- Ověřte, že uživatel používá aplikaci, která podporuje popisky citlivosti – viz [popisky](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)citlivosti v dokumentu .

- Pokud migrujete [popisky Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)uvědomte si důležité informace uvedené [tady.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Podpora ochrany před únikem informací o ztrátě dat: V současné době se jako podmínku v zásadách ochrany před únikem informací používejte jenom popisky uchovávání informací.  Podpora popisků citlivosti v zásadách ochrany před únikem informací zatím není dostupná, ale pracujeme na tom.

- Pokud je u popisku citlivosti povolené šifrování, můžete zvolit, jestli chcete:
    - Přiřazení oprávnění
    - Povolení uživatelům přiřazovat oprávnění


Další informace o možných problémech najdete v tématu [Známé problémy s popisky citlivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).