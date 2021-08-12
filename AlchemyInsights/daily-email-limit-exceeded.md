---
title: Byl překročen denní limit e-mailu. Pracovní postup je pozastavený.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914644"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Byl překročen denní limit e-mailu. Pracovní postup je pozastavený.

Tato chyba může být přijata v následujících situacích:

- Máte pracovní postup v SharePoint Online, který používá typ platformy SharePoint 2010 nebo SharePoint 2013.
- Pracovní postup je nakonfigurovaný tak, aby odesílal vlastní e-mailovou zprávu více než 200 uživatelům najednou, více než 10 000 příjemců za den nebo více než 30 zpráv za minutu.
- Když spustíte pracovní postup, e-mailová zpráva se neposílána a všimnete si následujícího chování:
    - U pracovního postupu s typem SharePoint platformy 2013 přejděte na **stránku Stav pracovního** postupu. Na stránce Stav pracovního postupu je interní **stav** nastavený na **Zahájeno** a informační bublina zobrazí Zprávu nelze **odeslat příjemci**.

Pokud chcete tento problém vyřešit, nakonfigurujte pracovní postup tak, aby odesílal e-mailové zprávy, aniž by Exchange Online [limity odesílatelů](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Můžete třeba použít pozastavení v pracovním postupu, poslat e-mail skupině Microsoft 365, distribuční skupině nebo skupině zabezpečení s podporou pošty nebo poslat zprávu méně než 200 příjemcům najednou.


Další informace najdete v následujícím [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Související témata
- [Vytvoření Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 