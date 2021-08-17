---
title: Čtení protokolů auditování odstraněných událostí
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896008"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Čtení protokolů auditování odstraněných událostí

Tady je postup:

1. Proveďte jednu z následujících akcí:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na **Audit** \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na portálu Microsoft 365 Defender přejděte <https://security.microsoft.com> na **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Pokud se zobrazí upozornění, že je potřeba tuto funkci zapnout, pokračujte a zapněte ji hned. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.

2. Na kartě **Hledání** na stránce **Auditování** nakonfigurujte následující nastavení:
   - **Rozsah dat a času:** V polích  Začátek a **Konec** vyberte rozsah dat a času.
   - **Aktivity:** Zadejte **Exchange poštovní schránky** a vyberte následující hodnoty:
     - **Odstraněné zprávy ze složky Odstraněná pošta**
     - **Přesunutí zpráv do složky Odstraněná pošta**

       Až budete hotovi, klikněte mimo podokno, abyste minimalizovali **podokno** Aktivity.

   - **Uživatelé:** Přijměte prázdnou výchozí hodnotu, aby se vrátily výsledky pro všechny uživatele, nebo zadejte jednoho nebo více uživatelů.

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.**

4. Výběrem aktivity ve výsledcích otevřete plovoucí okno podrobností. Další informace o odstraněné položce, jako je řádek předmětu a umístění položky při odstranění, se zobrazí v poli **AffectedItems.**

   > [!NOTE]
   > Odstraněné položky nemůžete obnovit pomocí funkce protokolu auditování. Pokud chcete obnovit odstraněné položky, podívejte se na stránku Obnovení odstraněných [e-mailových zpráv v Outlook na webu](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Další informace najdete v tématu Hledání v protokolu auditování a [prošetřování běžných problémů s podporou](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
