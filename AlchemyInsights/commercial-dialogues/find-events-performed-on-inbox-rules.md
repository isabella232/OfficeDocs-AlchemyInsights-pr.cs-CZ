---
title: Vyhledání událostí provedených s pravidly doručené pošty
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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058643"
---
# <a name="find-events-performed-on-inbox-rules"></a>Vyhledání událostí provedených s pravidly doručené pošty

Při vytváření, změně nebo odstranění pravidel doručené pošty se události zaznamenávají do protokolu auditování. Tady je postup, jak je zkontrolovat:

1. Přejděte do [Centra Office 365 zabezpečení & dodržování předpisů](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Vyberte Hledat > protokolu auditování.

    > [!NOTE]
    > Pokud se zobrazí oznámení, že je potřeba auditování zapnout, pokračujte a zapněte ho hned. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.
1. Vyberte pole Aktivity a najděte aktivity Exchange poštovní schránky a pak vyberte New-InboxRule vytvořit pravidlo doručené pošty z Outlook Web App. Až budete hotovi, klikněte mimo podokno, abyste minimalizovali podokno Aktivity.
1. Zadejte rozsah dat a potom v poli Uživatelé vyberte uživatelské jméno uživatele, kterého chcete prozkoumat. Můžete vybrat víc uživatelů najednou.
1. Vyberte Hledat. Aktivity se zobrazí v části Výsledky.
1. Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak vyberte Další informace. V části Parametry se zobrazí název pravidla, nastavené podmínky a akce, které pravidlo bude provádět.

Další informace najdete v článku Hledání Office 365 auditování a řešení běžných scénářů.