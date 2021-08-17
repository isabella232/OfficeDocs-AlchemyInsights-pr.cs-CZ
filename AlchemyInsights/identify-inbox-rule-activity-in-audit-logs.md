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
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891288"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Určení aktivity pravidla doručené pošty v protokolech auditování

Pomocí hledání v protokolu auditování v Centrum dodržování předpisů Microsoftu 365 zobrazit události pravidel doručené pošty (vytváření, úpravy a odstraňování pravidel doručené pošty).

1. Proveďte jeden z následujících kroků:
   - V Centrum dodržování předpisů Microsoftu 365 přejděte <https://compliance.microsoft.com> na **Audit** \> **řešení**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://compliance.microsoft.com/auditlogsearch> .
   - Na portálu Microsoft 365 Defender přejděte <https://security.microsoft.com> na **Audit**. Pokud chcete přejít přímo na **stránku Auditování,** použijte <https://security.microsoft.com/auditlogsearch> .

2. Na kartě **Hledání** na stránce **Auditování** nakonfigurujte následující nastavení:
   - **Rozsah dat a času:** V polích  Začátek a **Konec** vyberte rozsah dat a času.
   - **Aktivity:** Vyberte jednu nebo více z následujících hodnot:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Aktualizace pravidel doručené pošty z Outlook klienta**

3. Až skončíte, klikněte na **Hledat**. Aktivity se zobrazí na nové stránce **vyhledávání auditování.**

4. Výběrem aktivity ve výsledcích otevřete plovoucí okno podrobností. Informace o nastavení pravidla doručené pošty se zobrazí v **poli Parametry.**

Další informace najdete v tématu [Určení, jestli uživatel vytvořil pravidlo doručené pošty](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
