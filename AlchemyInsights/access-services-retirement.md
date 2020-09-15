---
title: Starobní služby Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698675"
---
# <a name="access-services-retirement"></a>Starobní služby Access Services

Jak jsme původně oznámili společnost Microsoft v MC97576, v březnu 2017 a pokračovali v komunikaci během minulého roku, jsou vyřazeny služby Access Services. Další fází tohoto procesu bude odebrání webových databází Accessu, které používají seznamy SharePointu jako odpovídající úložiště dat.

**Jak se to týká?**

Od června 2019 zastavíme vytváření nových Accessových databází v SharePointu Online a ukončete službu a všechny zbývající aplikace do dubna 2020.

**Co je potřeba udělat, abyste mohli připravit tuto změnu?**

Doporučujeme vytvořit plán přechodu pro webové databáze Accessu vaší organizace. Správci můžou pomocí [skeneru aplikace SharePoint pro Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) získat soupis aplikací pro Access, které weby používají.

Existuje několik způsobů migrace dat webových databází v Accessu:

- Import do místní databáze Accessu (. ACCDB) nebo na excelový soubor.
- Doporučujeme také prozkoumat Microsoft PowerApps jako alternativní platformu pro vytváření obchodních řešení pro webové a mobilní zařízení.