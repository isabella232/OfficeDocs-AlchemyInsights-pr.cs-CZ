---
title: Byl překročen denní limit e-mailu. Pracovní postup je pozastaven.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580326"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Byl překročen denní limit e-mailu. Pracovní postup je pozastaven.

Tato chyba může být přijata v následujících scénářích:

- V SharePointu Online máte pracovní postup, který používá typ platformy pracovního postupu SharePointu 2010 nebo SharePointu 2013.
- Pracovní postup je nakonfigurován tak, aby odesílá vlastní e-mailovou zprávu více než 200 uživatelům najednou, více než 10 000 příjemcům denně nebo více než 30 zpráv za minutu.
- Při spuštění pracovního postupu se e-mailová zpráva neodesílá a zjistíte následující chování:
    - U pracovního postupu s typem platformy SharePointu 2013 přejděte na stránku **Stav pracovního postupu.** Na stránce Stav pracovního postupu je **vnitřní stav** nastaven na **počáteční**hodnotu a v bublině informace se zobrazí možnost **Nelze odeslat příjemci**.

Chcete-li tento problém vyřešit, nakonfigurujte pracovní postup tak, aby odesílal e-mailové zprávy bez překročení [limitů odesílatele Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Můžete například použít pozastavení v pracovním postupu, odeslat e-mail skupině Microsoft 365, distribuční skupině nebo skupině zabezpečení s povolenou poštou nebo odeslat zprávu méně než 200 příjemcům najednou.


Další informace naleznete v následujícím [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Související témata
- [Vytvořit tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 