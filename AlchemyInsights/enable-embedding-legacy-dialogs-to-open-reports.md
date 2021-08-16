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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003382"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Povolení vkládání zastaralých dialogů pro otevření sestav

**Příznak**

Uživatelům se nedaří otevřít sestavy. „Došlo k nějakému problému. Další informace najdete v technických podrobnostech.“

**Příčina**

Sestavy se nedaří načíst do nástroje UCI a zobrazuje se chybová zpráva: „Popisovač formuláře je null nebo není definovaný.“ Sestavy v nástroji UCI vyžadují starší verze dialogů, takže systém zákazníka musí mít povolenou funkci *allowlegacydialogsembedding*.

**Řešení**

1. Přejděte na **Nastavení > Správa > Nastavení systému > karta Obecné**.

2. Nastavte možnost „Povolí vkládání určitých zastaralých dialogů do klienta prohlížeče Sjednoceného rozhraní“ na **Ano**.
