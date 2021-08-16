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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028724"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Určení, kdy je v poštovních schránkách nakonfigurované externí přeposílání e-mailů

Když Microsoft 365 externí přeposílání e-mailů v poštovní schránce, aktivita se audituje jako součást rutiny **Set-Mailbox.** Aktivitu můžete zobrazit pomocí vyhledávání v protokolu auditování v Centru & dodržování předpisů.

1. Přihlaste se do [centra Microsoft 365 dodržování předpisů](https://protection.office.com/).

2. Přejděte na **vyhledávací stránku protokolu**  >  **auditování** hledání.

3. Vyberte rozsah dat v **polích Počáteční datum** a **Koncové** datum. Nemusíte zadít uživatelské jméno. Ověřte, **jestli je** pole Aktivity nastavené na Zobrazit výsledky pro všechny **aktivity**.

4. Klikněte na **Hledat.**

Ve výsledcích klikněte na **Filtrovat výsledky** **a** do pole filtru aktivity zadejte Nastavit poštovní schránku. Ve výsledcích vyberte záznam auditování. V **informačním podokně Podrobnosti** klikněte na **Další informace**. Abyste zjistili, jestli aktivita souvisí s přeposíláním e-mailů, musíte se podívat na podrobnosti jednotlivých záznamů auditování.

- **Id Objektu:** Hodnota aliasu poštovní schránky, která byla změněna.

- **Parametry:** _ForwardingSmtpAddress_ označuje cílovou e-mailovou adresu.

- **Id_uživatele:** Uživatel, který nakonfiguroval přeposílání e-mailů v poštovní schránce v **poli Id Objektu.**

Další informace najdete v článku [Určení, kdo nastavil přeposílání e-mailů pro poštovní schránku](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
