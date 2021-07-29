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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630170"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Určení aktivity pravidla doručené pošty v protokolech auditování

K zobrazení událostí pravidel doručené pošty (vytváření, úpravy a odstraňování pravidel doručené pošty) můžete použít vyhledávání v protokolu auditování v centru Microsoft 365 Security & Compliance Center.

1. Přihlaste se do [centra Microsoft 365 dodržování předpisů](https://protection.office.com/).

2. Přejděte na **vyhledávací stránku protokolu**  >  **auditování** hledání.

3. Vyberte rozsah dat v **polích Počáteční datum** a **Koncové** datum.

4. V **Exchange aktivity poštovní** schránky  ověřte, jestli je pole Aktivity nastavené na **New-InboxRule Create/modify/enable/disable inbox rule**.

5. Klikněte na **Hledat.**

Ve výsledcích vyberte záznam auditování. V informačním podokně podrobností klikněte na **Další informace**. Informace o nastavení pravidla doručené pošty se zobrazí v **poli Parametry.**

Další informace najdete v článku [Určení, jestli uživatel vytvořil pravidlo doručené pošty.](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
