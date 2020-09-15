---
title: Ve výsledcích hledání SharePointu se nezobrazuje obsah
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713123"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Ve výsledcích hledání SharePointu se nezobrazuje obsah

Pokud se ve výsledcích hledání nezobrazuje očekávaný obsah, postupujte podle těchto kroků:
  
1. Zkontrolujte, jestli je **Web** obsahující očekávaný obsah nastavený tak, aby se obsah zobrazoval ve výsledcích hledání. Postupujte podle pokynů v tématu [zobrazení obsahu na webu ve výsledcích hledání](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Zkontrolujte, jestli je **seznam** nebo **Knihovna** obsahující očekávaný obsah nastavená tak, aby se obsah zobrazil ve výsledcích hledání. Postupujte podle pokynů v tématu [zobrazení obsahu ze seznamů nebo knihoven ve výsledcích hledání](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Ověřte, že je stránka, dokument nebo vlastní rozložení stránky publikované jako **hlavní verze.** Postup při kroku 3 v [hledání nevrací všechny výsledky v SharePointu Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Ověřte, jestli má uživatel **oprávnění** k zobrazení obsahu. Postupujte podle pokynů v tématu [Principy úrovní oprávnění v SharePointu](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Pokud se změnilo schéma vyhledávání přidáním nové spravované vlastnosti, upraví spravovanou vlastnost nebo odebráním spravované vlastnosti, která vyžaduje procházení a přeindexování. **Znovu Indexujte** obsah podle pokynů v tématu [Ruční procházení a přeindexování webu, knihovny nebo seznamu](https://docs.microsoft.com/sharepoint/crawl-site-content). To může nějakou dobu trvat a až 24 hodin znovu zkontrolujte výsledky.

Další informace najdete v tématu [Povolení vyhledávání obsahu na webu](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
