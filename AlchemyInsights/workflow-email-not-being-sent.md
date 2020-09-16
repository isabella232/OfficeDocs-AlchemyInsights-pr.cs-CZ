---
title: E-mail pracovního postupu se neposílá
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748982"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail pracovního postupu se neposílá pro seznam nebo knihovnu SharePointu

1. E-mail od pracovních postupů se neposílá všem uživatelům nebo jenom určitým uživatelům, nebo se zobrazí chyba **: e-mailovou zprávu nelze odeslat. Zkontrolujte, jestli má e-mail platného příjemce**.

    Zkontrolujte, jestli uživatel existuje ve skupině oprávnění **všech lidí** (seznam informací o uživateli) pro tuto kolekci webů.  Ukázka přímé adresy URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Pokud uživatel neexistuje, zkontrolujte, jestli je uživatel přihlášený na stránku. 
    - Pokud je to externí uživatel, ujistěte se, že Pozvánka byla přijata.
    - Pokud uživatel ve skupině oprávnění existuje, zkontrolujte správnost e-mailové adresy.
    - Pokud tady není nastavená e-mailová adresa uživatele, vytvořte pro tohoto uživatele ukázkové upozornění, které vynutí synchronizaci tohoto uživatelského účtu z profilů uživatelů SharePointu do této kolekce webů.
 
2. E-maily od pracovních postupů se odesílají správcům kolekce webů, ale ne ostatním uživatelům a zobrazují se vám chybové zprávy **http <span>:</span>//URL/_vti_bin/Client.XVC.SP.Utilities.Utility.SendEmail**.
 

    [Pokud odešlete e-mail skupině SharePointu](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups), přečtěte si článek přístup odepřen.

    Ověřte také, že funkce kolekce webů **režimu uzamčení oprávnění uživatelů s omezeným přístupem** není aktivní.


## <a name="related-topics"></a>Související témata
Chcete vyzkoušet tok Microsoftu v SharePointu Online?
- [Vytvoření toku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


