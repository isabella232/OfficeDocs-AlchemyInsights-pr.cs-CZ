---
title: Byl překročen denní limit pro e-mail. Pracovní postup je pozastaven.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731556"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Byl překročen denní limit pro e-mail. Pracovní postup je pozastaven.

Tato chyba se zobrazí v následujících situacích:

- V SharePointu Online máte pracovní postup používající typ platformy SharePoint 2010 nebo SharePoint 2013 pracovního postupu.
- Pracovní postup je nakonfigurovaný tak, aby posílal vlastní e-mailovou zprávu více než 200 uživatelům najednou, více než 10 000 příjemců za den nebo více než 30 zpráv za minutu.
- Po spuštění pracovního postupu se e-mailová zpráva neodešle a všimnete si následujícího chování:
    - U pracovního postupu s typem platformy SharePoint 2013 přejděte na stránku **stav pracovního postupu** . Na stránce Stav pracovního **postupu je nastaven stav** **aktivní na zahájeno**a informační bublina **nemůže odeslat příjemci**.

Pokud chcete tento problém vyřešit, nakonfigurujte pracovní postup tak, aby odesílal e-mailové zprávy bez překročení [limitů odesílatelů Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Můžete například použít příkaz pozastavit v pracovním postupu, odeslat e-mail skupině Microsoft 365, skupině zabezpečení s povoleným e-mailem nebo zaslat zprávu na méně než 200 příjemců najednou.


Další informace najdete v následujícím [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Související témata
- [Vytvoření toku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 