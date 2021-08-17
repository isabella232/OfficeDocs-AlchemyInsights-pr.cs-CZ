---
title: Obsah se nezobrazuje ve výsledcích SharePoint hledání
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
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081603"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Obsah se nezobrazuje ve výsledcích SharePoint hledání

Pokud se očekávaný obsah ve výsledcích hledání nezobrazuje, postupujte takto:
  
1. Zkontrolujte, **že je web,** který obsahuje očekávaný obsah, nastavený tak, aby se obsah ve výsledcích hledání objevil. Postupujte podle pokynů v [části Zobrazení obsahu na webu ve výsledcích hledání](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Zkontrolujte, **že je seznam** **nebo knihovna** obsahující očekávaný obsah nastavený tak, aby se obsah ve výsledcích hledání objevil. Postupujte podle pokynů v článku [Zobrazení obsahu ze seznamů nebo knihoven ve výsledcích hledání.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Ověřte, jestli je rozložení stránky, dokumentu nebo vlastního rozložení stránky publikované jako **hlavní verze.** Postupujte podle kroku 3 ve vyhledávání nevrátí všechny výsledky v [SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Ověřte, jestli má **uživatel oprávnění** k zobrazení obsahu. Postupujte podle pokynů v [tématu Principy úrovní oprávnění v SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Pokud se schéma hledání změnilo přidáním nové spravované vlastnosti, úpravou spravované vlastnosti nebo odebráním spravované vlastnosti, bude potřeba požádat o procházení a opětovné indexování. **Obsah můžete znovu** indexovat podle pokynů v článku Ruční vyžádání procházení [a opětovné indexování webu, knihovny nebo seznamu.](https://docs.microsoft.com/sharepoint/crawl-site-content) Může to chvíli trvat, počkejte 24 hodin, než znovu zkontrolujte výsledky.

Další informace najdete v tématu Povolení prohledávatelného obsahu [na webu.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
