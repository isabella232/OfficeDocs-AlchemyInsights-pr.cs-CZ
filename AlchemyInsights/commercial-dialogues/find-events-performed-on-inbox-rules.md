---
title: Hledání událostí provedených u pravidel doručené pošty
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481275"
---
# <a name="find-events-performed-on-inbox-rules"></a>Hledání událostí provedených u pravidel doručené pošty

Když pravidla doručené pošty vytváříte, měníte nebo odstraníte, zaznamenávají se události do protokolu auditování. Tady je postup, jak je zkontrolovat:

1. Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 & dodržování předpisů.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vyberte Hledat > v protokolu auditování.

    > [!NOTE]
    > Pokud vidíte oznámení, že je potřeba auditování zapnout, můžete ho teď zapnout. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.
1. Vyberte pole Aktivity, najděte aktivity poštovní schránky Exchange a pak vyberte New-InboxRule vytvořit pravidlo doručené pošty z Outlook Web Appu. Až budete hotovi, kliknutím mimo podokno podokno aktivit minimalizujte.
1. Zadejte rozsah dat a pak v poli Uživatelé vyberte uživatelské jméno uživatele, kterého chcete prozkoumat. Můžete vybrat víc uživatelů najednou.
1. Vyberte Hledat. Aktivity se zobrazí v části Výsledky.
1. Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak vyberte Další informace. V části Parametry můžete vidět název pravidla, sadu podmínek a akce, které bude pravidlo provádět.

Další informace najdete v protokolu auditování Office 365, kde najdete řešení běžných scénářů.