---
title: Problémy s výkonem SharePoint nebo OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911835"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint nebo OneDrive, nepřístupné nebo nedostupné pro více uživatelů

SharePoint nebo OneDrive mohou být pomalé, nepřístupné nebo nedostupné nebo 503 chyb z několika důvodů zobrazit nedostupné služby nebo 503 chyb:
  
- Pokud je váš SharePoint nebo OneDrive pro více uživatelů pomalý nebo zpožděný, může dojít k dočasnému problému se službou, kdy se uživatelům při přístupu k SharePoint webu nebo obsahu OneDrive navigace. Podívejte se [na řídicí panel Stavu služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) a podívejte se, jestli má vaše organizace vliv.
  
- Uživatelé mohou při pokusu o přechod na SharePoint nebo OneDrive *503* serveru. Tato chyba může být způsobena omezením v rámci SharePoint služby. SharePoint Online využívá omezování k zajištění optimálního výkonu a spolehlivosti svých služeb. Omezování limituje počet akcí uživatelů nebo současných volání (podle skriptů nebo kódu), aby nedocházelo k nadměrnému využití prostředků. Další informace o omezení najdete v tématu Vyhněte se omezení nebo zablokování SharePoint [Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Pokud u klasického  nebo moderního webu nebo stránky **SharePoint** nízký výkon, analyzujte stránky pomocí nástroje [Diagnostika](https://aka.ms/perftool) stránky.
  
- Pokud stále dochází k obecnému pomalému výkonu, přečtěte si informace v dolní části tohoto článku: Úvod k ladění výkonu pro [SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  