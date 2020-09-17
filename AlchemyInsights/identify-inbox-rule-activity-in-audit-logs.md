---
title: Určení aktivity pravidla doručené pošty v protokolech auditování
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779044"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Určení aktivity pravidla doručené pošty v protokolech auditování

Pokud chcete zobrazit události pravidla doručené pošty (vytváření, úpravy a odstraňování pravidel doručené pošty), můžete použít vyhledávání v protokolu auditování v centru & zabezpečení Microsoft 365.

1. Přihlaste se do [centra zabezpečení Microsoft 365 Security &](https://protection.office.com/).

2. Přejděte na stránku **Search**pro  >  **vyhledávání protokolu auditování** .

3. V polích **Datum zahájení** a **Datum ukončení** vyberte rozsah dat.

4. V části **aktivity poštovní schránky Exchange**ověřte, že pole **aktivity** je nastavené na **New-InboxRule**.

5. Klikněte na **Hledat**.

Ve výsledcích vyberte záznam auditu. V rozevíracím seznamu podrobností klikněte na **Další informace**. Informace o nastavení pravidla doručené pošty se zobrazí v poli **parametry** .

Další informace najdete v tématu [určení, jestli uživatel vytvořil pravidlo doručené pošty](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .
