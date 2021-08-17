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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313492"
---
# <a name="find-events-performed-on-inbox-rules"></a>Vyhledání událostí provedených s pravidly doručené pošty

Při vytváření, změně nebo odstranění pravidel doručené pošty se události zaznamenávají do protokolu auditování. Tady je postup, jak je zkontrolovat:

1. Proveďte jednu z následujících akcí:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na Audit  \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na Microsoft 365 Defender přejděte na <https://security.microsoft.com> **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://security.microsoft.com/auditlogsearch> .

    **Poznámka:** Pokud se zobrazí upozornění, že je potřeba auditování zapnout, pokračujte a zapněte ho hned. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.
1. Vyberte pole Aktivity a najděte aktivity Exchange poštovní schránky a pak vyberte New-InboxRule vytvořit pravidlo doručené pošty z Outlook Web App. Až budete hotovi, klikněte mimo podokno, abyste minimalizovali podokno Aktivity.
1. Zadejte rozsah dat a potom v poli Uživatelé vyberte uživatelské jméno uživatele, kterého chcete prozkoumat. Můžete vybrat víc uživatelů najednou.
1. Vyberte Hledat. Aktivity se zobrazí v části Výsledky.
1. Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak vyberte Další informace. V části Parametry se zobrazí název pravidla, nastavené podmínky a akce, které pravidlo bude provádět.

2. Na kartě **Hledání** na stránce **Auditování** nakonfigurujte následující nastavení:
   - **Rozsah dat a času:** V polích  Začátek a **Konec** vyberte rozsah dat a času.
   - **Aktivity:** Vyberte **New-InboxRule Create inbox rule from Outlook Web App**

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.**

4. Výběrem aktivity ve výsledcích otevřete plovoucí okno podrobností. V části **Parametry** se zobrazí název pravidla, nastavené podmínky a akce, které pravidlo bude provádět.

Další informace najdete v tématu [Hledání v protokolu auditování a prošetřování běžných problémů s podporou](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
