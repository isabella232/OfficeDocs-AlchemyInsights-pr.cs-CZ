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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317801"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Zjistěte, kdo nastavil přeposílání poštovní schránky a jak

Pokud bylo u poštovní schránky nastavené externí přeposílání, aktivita se audituje jako součást rutiny **Set-Mailbox.** Tady je postup, jak najít aktivitu v protokolu auditování:

1. Proveďte jednu z následujících akcí:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na Audit  \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na Microsoft 365 Defender přejděte na <https://security.microsoft.com> **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://security.microsoft.com/auditlogsearch> .

   **Poznámka:** Pokud se zobrazí upozornění, že je potřeba auditování zapnout, pokračujte a zapněte ho hned. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.

2. Na stránce **Auditování** ověřte, že **je vybraná karta** Hledání, a nakonfigurujte následující nastavení:
   - V polích Začátek a  Konec vyberte rozsah dat a **času.**
   - Ověřte, **že pole Aktivity** obsahuje zobrazit výsledky pro všechny **aktivity**.

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.**

4. Ve výsledcích kliknutím na sloupec **Aktivita** seřadíte výsledky a vyhledejte položky **Sady poštovních** schránek.

5. Výběrem aktivity ve výsledcích otevřete plovoucí okno podrobností. Abyste zjistili, jestli aktivita souvisí s přeposíláním e-mailů, musíte se podívat na podrobnosti jednotlivých záznamů auditování:
   - **Id Objektu:** Hodnota aliasu poštovní schránky, která byla změněna.
   - **Parametry:** _ForwardingSmtpAddress_ označuje cílovou e-mailovou adresu.
   - **Id_uživatele:** Uživatel, který nakonfiguroval přeposílání e-mailů v poštovní schránce v **poli Id Objektu.**

Další informace najdete v článku [Určení, kdo nastavil přeposílání e-mailů pro poštovní schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
