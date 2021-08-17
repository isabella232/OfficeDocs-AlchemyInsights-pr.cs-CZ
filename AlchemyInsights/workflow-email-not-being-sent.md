---
title: E-mail pracovního postupu se neposílán
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
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072513"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail pracovního postupu se neposílán pro SharePoint nebo knihovnu

1. E-maily z pracovních postupů se neposílaly všem uživatelům ani jenom konkrétním uživatelům nebo se zobrazí chybová zpráva E-mailová zpráva nemůže být odeslána. Ujistěte se, že **e-mail má platného příjemce.**

    Zkontrolujte, jestli uživatel  pro kolekci webů existuje ve skupině Oprávnění všichni lidé (seznam informací o uživateli).  Ukázková přímá adresa URL: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Pokud uživatel neexistuje, ujistěte se, že je uživatel přihlášený ke stránce. 
    - Pokud se jedná o externího uživatele, ujistěte se, že pozvánka byla přijata.
    - Pokud uživatel ve skupině oprávnění existuje, zkontrolujte, jestli je e-mailová adresa správná.
    - Pokud tady není nastavená e-mailová adresa uživatelů, vytvořte pro tohoto uživatele ukázkové upozornění, které vynutí synchronizaci tohoto uživatelského účtu z profilů uživatelů SharePoint do této kolekce webů.
 
2. E-maily z pracovních postupů se posílají správcům kolekce webů, ale ne jiným uživatelům a zobrazí se chybová zpráva **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Informace najdete v tématu Přístup odepřen při odeslání [e-mailu SharePoint skupině.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Ověřte také,  že funkce kolekce webů v režimu uzamčení oprávnění uživatele s omezeným přístupem není aktivní.


## <a name="related-topics"></a>Související témata
Chcete vyzkoušet Microsoft Flow SharePoint Online?
- [Vytvoření Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


