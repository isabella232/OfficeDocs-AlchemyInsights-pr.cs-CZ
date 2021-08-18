---
title: Prozkoumat aktivity všech uživatelů
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332336"
---
# <a name="investigate-all-the-users-activities"></a>Prozkoumat aktivity všech uživatelů

Tady je postup:

1. Proveďte jednu z následujících akcí:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na Audit  \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na Microsoft 365 Defender přejděte na <https://security.microsoft.com> **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://security.microsoft.com/auditlogsearch> .

    **Poznámka:** Pokud se zobrazí upozornění, že je potřeba tuto funkci zapnout, pokračujte a zapněte ji hned. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.

2. Na kartě **Hledání** na stránce **Auditování** nakonfigurujte následující nastavení:
   - **Rozsah dat a času:** V polích  Začátek a **Konec** vyberte rozsah dat a času.
   - **Aktivity:** Pokud vás zajímá určitá aktivita, vyberte ji ze seznamu. v opačném případě vrátí výchozí hodnota **Zobrazit výsledky pro všechny aktivity** všechny aktivity.
   - **Uživatelé:** Přijměte prázdnou výchozí hodnotu, aby se vrátily výsledky pro všechny uživatele, nebo zadejte jednoho nebo více uživatelů.

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.** Zobrazí se **IP adresa**, **Uživatel** a **Název** aktivity.

4. Pokud chcete stáhnout výsledky, vyberte **Exportovat** \> **stáhnout všechny výsledky**.

5. Výběrem aktivity ve výsledcích otevřete plovoucí okno podrobností.

Další informace najdete v tématu [Hledání v protokolu auditování a prošetřování běžných problémů s podporou](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
