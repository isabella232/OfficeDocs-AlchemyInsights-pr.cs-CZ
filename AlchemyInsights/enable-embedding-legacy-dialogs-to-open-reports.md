---
title: Povolení vkládání zastaralých dialogů pro otevření sestav
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814257"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Povolení vkládání zastaralých dialogů pro otevření sestav

**Příznak**

Uživatelům se nedaří otevřít sestavy. „Došlo k nějakému problému. Další informace najdete v technických podrobnostech.“

**Příčina**

Sestavy se nedaří načíst do nástroje UCI a zobrazuje se chybová zpráva: „Popisovač formuláře je null nebo není definovaný.“ Sestavy v nástroji UCI vyžadují starší verze dialogů, takže systém zákazníka musí mít povolenou funkci *allowlegacydialogsembedding*.

**Řešení**

1. Přejděte na **Nastavení > Správa > Nastavení systému > karta Obecné**.

2. Nastavte možnost „Povolí vkládání určitých zastaralých dialogů do klienta prohlížeče Sjednoceného rozhraní“ na **Ano**.
