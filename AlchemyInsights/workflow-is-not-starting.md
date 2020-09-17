---
title: Pracovní postup se nespouští
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794760"
---
# <a name="workflow-is-not-starting"></a>Pracovní postup se nespouští

- SharePoint 2010 a SharePoint 2013 pracovní postupy se nespouštějí.

    - Pokud se váš pracovní postup nespouští, může se jednat o dočasný problém s poskytováním služeb, při kterém mohou uživatelé zaznamenat přerušované zpoždění pomocí pracovního postupu. Podívejte se na [řídicí panel stavu služeb](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) a zjistěte, jestli je vaše organizace ovlivněná.

    - Pokud od prvního vystavení tohoto problému uplynulo více než 24 hodin, protokolujte lístek podpory. V mnoha případech jsme na řešení ještě pracujeme. Dokončete řešení alespoň 24 hodin.

- Zpožděné zahájení pracovních postupů SharePoint 2010

    - K tomu dojde, pokud je pracovní postup spuštěn ve velkých dávkách. (například když se přidají několik položek najednou)

    - Pracovní postupy nejsou navržené pro spuštění v reálném čase, takže zpoždění se provádí podle chování.

   -  Pokud je pracovní postup komplexní jazyk XML (Extensible Object Markup Language), může být kompilace pomalé. Podívejte se na [Tento](https://support.microsoft.com//kb/3043697) článek.

    - Pracovní postup byste měli zjednodušit nebo ho přenavrhovat pomocí typu platformy Microsoft SharePoint 2013 Workflow.

    - Pokud se vaše historie pracovního postupu zvětšila, můžete položky vymazat nebo vytvořit nový seznam historie.

        Další informace: [vymazání historie pracovního postupu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Související témata
Chcete vyzkoušet tok Microsoftu v SharePointu Online?
- [Vytvoření toku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


