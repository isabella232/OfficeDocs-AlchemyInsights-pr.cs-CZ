---
title: Pracovní postup se nezahajuje.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403736"
---
# <a name="workflow-is-not-starting"></a>Pracovní postup se nezahajuje.

- Pracovní postupy SharePointu 2010 a SharePointu 2013 se nezahajuje.

    - Pokud pracovní postup nezačáte, může docházet k dočasnému problému se službou, kdy se uživatelům může při průběhu pracovního postupu občas vyskytnout zpoždění. Zkontrolujte řídicí [panel Stavu služby](https://admin.microsoft.com/AdminPortal/Home/servicehealth) a podívejte se, jestli má vaše organizace vliv.

    - Pokud od prvního pohledu na tento problém uplynulo více než 24 hodin, přihlaste se prosím k lístku podpory. V mnoha případech už pracujeme na řešení. Na dokončení řešení nám prosím dejte aspoň 24 hodin.

- Pracovní postupy SharePointu 2010 se zpozdí při spuštění.

    - K tomu dochází, pokud se pracovní postup aktivuje ve velkých dávkách. (například když se přidá několik položek najednou).

    - Pracovní postupy nejsou navržené tak, aby spouštěly v reálném čase, takže zpoždění je chování podle návrhu.

   -  Pokud je pracovní postup složitý, může být kompilace pomalá. Podívejte [se na tento](https://support.microsoft.com//kb/3043697) článek.

    - Pracovní postup byste měli zjednodušit nebo ho předělat pomocí typu platformy Microsoft SharePoint 2013 Workflow.

    - Pokud se historie pracovních postupů rozrostla, možná budete chtít položky vymazat nebo vytvořit nový seznam historie.

        Další informace: [Vymazání historie pracovních postupů](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Související témata
Chcete vyzkoušet Microsoft Flow v SharePointu Online?
- [Vytvoření toku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
