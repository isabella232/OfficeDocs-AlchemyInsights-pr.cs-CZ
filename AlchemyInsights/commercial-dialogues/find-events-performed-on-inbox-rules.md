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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882628"
---
# <a name="find-events-performed-on-inbox-rules"></a>Vyhledání událostí provedených s pravidly doručené pošty

Při vytváření, změně nebo odstranění pravidel doručené pošty se události zaznamenávají do protokolu auditování. Tady je postup, jak je zkontrolovat:

1. Proveďte jednu z následujících akcí:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na **Audit** \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na portálu Microsoft 365 Defender přejděte <https://security.microsoft.com> na **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Pokud se zobrazí oznámení, že je potřeba auditování zapnout, pokračujte a zapněte ho hned. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.

2. Na kartě **Hledání** na stránce **Auditování** nakonfigurujte následující nastavení:
   - **Rozsah dat a času:** V polích  Začátek a **Konec** vyberte rozsah dat a času.
   - **Aktivity:** **Vyberte New-InboxRule Create inbox rule from Outlook Web App**

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.**

4. Výběrem aktivity ve výsledcích otevřete plovoucí okno podrobností. V části **Parametry** se zobrazí název pravidla, nastavené podmínky a akce, které pravidlo bude provádět.

Další informace najdete v tématu [Hledání v protokolu auditování a prošetřování běžných problémů s podporou](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
