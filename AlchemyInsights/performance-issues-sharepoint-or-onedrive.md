---
title: Problémy s výkonem – SharePoint nebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771894"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint nebo OneDrive pomalý, nedostupný ani nedostupný pro víc uživatelů

SharePoint nebo OneDrive můžou být pomalé, nepřístupné nebo nedostupné nebo nemusí být zobrazovat 503 služby, a to z několika důvodů:
  
- Pokud je váš web SharePointu nebo OneDrivu pomalý nebo opožděný pro víc uživatelů, může se jednat o dočasný problém s tím, že uživatelé při přístupu k SharePointovým webům nebo obsahu OneDrivu zastupují. Podívejte se na [řídicí panel stavu služeb](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) a zjistěte, jestli je vaše organizace ovlivněná.
  
- Při pokusu o přechod na weby SharePointu nebo OneDrivu může dojít k chybě *serveru 503* . Tato chyba může být způsobena omezením služby SharePoint. SharePoint Online využívá omezování k zajištění optimálního výkonu a spolehlivosti svých služeb. Omezování limituje počet akcí uživatelů nebo současných volání (podle skriptů nebo kódu), aby nedocházelo k nadměrnému využití prostředků. Další informace o omezování najdete [v článku Neomezovat nebo zablokovat v SharePointu Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Pokud se setkáte s nízkým výkonem při používání **klasického** nebo **moderního** webu nebo stránky SharePointu, analyzujte stránky pomocí [nástroje Diagnostika stránky](https://aka.ms/perftool) .
  
- Pokud pořád dochází k obecnému snížení výkonu, podívejte se na materiály v dolní části tohoto článku: [Úvod k ladění výkonu pro SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  