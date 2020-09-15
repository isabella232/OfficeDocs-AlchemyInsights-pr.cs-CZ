---
title: Identifikace externího předávání e-mailů u poštovních schránek v protokolech auditování
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696290"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Určení, kdy je u poštovních schránek nakonfigurovaný externí e-mail

Když uživatel Microsoft 365 nakonfiguruje externí předávání e-mailů v poštovní schránce, bude auditována jako součást rutiny **Set-Mailbox** . Aktivitu můžete zobrazit pomocí vyhledávání v protokolu auditování & centru dodržování předpisů.

1. Přihlaste se do [centra zabezpečení Microsoft 365 Security &](https://protection.office.com/).

2. Přejděte na stránku **Search**pro  >  **vyhledávání protokolu auditování** .

3. V polích **Datum zahájení** a **Datum ukončení** vyberte rozsah dat. Nemusíte zadávat uživatelské jméno. Ověřte, jestli je pole **aktivity** nastaveno tak, aby **zobrazovalo výsledky pro všechny aktivity**.

4. Klikněte na **Hledat**.

Ve výsledcích klikněte v poli Filtr aktivity na filtrovat **výsledky** a typ **Nastavení – poštovní schránka** . Ve výsledcích vyberte záznam auditu. V rozevíracím seznamu **podrobností** klikněte na **Další informace**. Pokud chcete zjistit, jestli aktivita souvisí s přesměrováním e-mailu, podívejte se na podrobnosti o jednotlivých záznamech auditu.

- **ObjectID**: hodnota aliasu poštovní schránky, která byla změněna.

- **Parametry**: _ForwardingSmtpAddress_ označuje cílovou e-mailovou adresu.

- **UserID**: uživatel, který nakonfigurovali přesměrování e-mailu na poštovní schránku v poli **objectID**

Další informace najdete v tématu [určení, kdo nastavil přeposlání e-mailů pro poštovní schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
