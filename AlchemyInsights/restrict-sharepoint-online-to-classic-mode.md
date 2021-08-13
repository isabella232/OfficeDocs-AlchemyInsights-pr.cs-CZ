---
title: Omezení SharePoint Online na klasický režim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958794"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Omezení SharePoint Online na klasický režim

Některé organizace pořád vyžadují klasické režimové prostředí. I když neexistují žádné plány na odebrání klasického režimu na granulární úrovni, už není možné omezit celou organizaci (tenanta) na klasický režim pro seznamy a knihovny.

Správce bude mít následující možnosti pro správu jednotlivých seznamů a knihoven v klasickém režimu pomocí granulovaných přepínačů výslovného odhlášení, které poskytujeme na následujících úrovních:

- Kolekce webů
- web
- seznam
- knihovna

Seznamy, které používají určité funkce a přizpůsobení, které moderní technologie nepodporují, se navíc automaticky přepne do klasického režimu.

Od 1. dubna 2019 začne proces zakázání odhlášení z moderního seznamu a knihoven na úrovni tenanta a bude pokračovat do 31. května 2019.  Seznamy a knihovny, které jsou v klasickém režimu v důsledku odhlášení tenanta, se automaticky přesunou na moderní.

Pokud potřebujete klasický režim, [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) přečtěte si tady další [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) informace a pokyny k powershellu PnP, které popisují možnosti a nástroje, které můžete dnes použít k použití klasického režimu.
