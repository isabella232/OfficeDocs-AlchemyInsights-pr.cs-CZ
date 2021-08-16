---
title: Zjistěte, kdo nastavil přeposílání poštovní schránky a jak
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988172"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Zjistěte, kdo nastavil přeposílání poštovní schránky a jak

Pokud bylo u poštovní schránky nastavené externí přeposílání, aktivita se audituje jako součást Set-Mailbox rutiny. Tady je postup, jak najít aktivitu v protokolu auditování:

1. Přejděte do [Centra Office 365 zabezpečení & dodržování předpisů](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Vyberte **Hledat** >  **v protokolu auditování**.
    > [!NOTE]
    > Pokud se zobrazí oznámení, že je potřeba auditování zapnout, pokračujte a zapněte ho hned. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.
1. Ujistěte **se, že** je pole Aktivity nastavené na **Zobrazit výsledky pro všechny aktivity** (výchozí). Zadejte rozsah dat. Nemusíte zadít uživatelské jméno.
1. Vyberte **Hledat**. Aktivity se zobrazí v části **Výsledky**.
1. Vyberte **Filtrovat výsledky** a potom do pole Filtr aktivity zadejte Nastavit **poštovní** schránku.  Tím se vrátí všechny **aktivity set-mailboxu.**
1. Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak vyberte **Další informace**. V **části Parametry** se zobrazí e-mailová adresa pro přeposílání nastavená v poštovní schránce. **Id_uživatele** představuje uživatele, který nastavil externí přeposílání poštovní schránky.
Další informace najdete v tématu Hledání v Office 365 auditování a [řešení běžných scénářů](https://go.microsoft.com/fwlink/?linkid=2103944).