---
title: Určení externího přeposílání e-mailů u poštovních schránek v protokolech auditování
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331152"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Určení, kdy je v poštovních schránkách nakonfigurované externí přeposílání e-mailů

Když Microsoft 365 externí přeposílání e-mailů v poštovní schránce, aktivita se audituje jako součást rutiny **Set-Mailbox.** Aktivitu můžete zobrazit pomocí vyhledávání v protokolu auditování. Tady je postup.

1. Proveďte jeden z následujících kroků:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na Audit  \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na Microsoft 365 Defender přejděte na <https://security.microsoft.com> **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://sip.security.microsoft.com/auditlogsearch> .

2. Na stránce **Auditování** ověřte, že **je vybraná karta** Hledání, a nakonfigurujte následující nastavení:
   - V polích Začátek a  Konec vyberte rozsah dat a **času.**
   - Ověřte, **že pole Aktivity** obsahuje zobrazit výsledky pro všechny **aktivity**.

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.**

4. Ve výsledcích klikněte na **Filtrovat výsledky** **a** do pole filtru aktivity zadejte Nastavit poštovní schránku.

5. Ve výsledcích vyberte záznam auditování. V **informačním podokně Podrobnosti** klikněte na **Další informace**. Abyste zjistili, jestli aktivita souvisí s přeposíláním e-mailů, musíte se podívat na podrobnosti jednotlivých záznamů auditování.

   - **Id Objektu:** Hodnota aliasu poštovní schránky, která byla změněna.
   - **Parametry:** _ForwardingSmtpAddress_ označuje cílovou e-mailovou adresu.
   - **Id_uživatele:** Uživatel, který nakonfiguroval přeposílání e-mailů v poštovní schránce v **poli Id Objektu.**

Další informace najdete v článku [Určení, kdo nastavil přeposílání e-mailů pro poštovní schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
