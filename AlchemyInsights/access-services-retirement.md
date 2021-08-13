---
title: Vyřazení služeb accessu
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938688"
---
# <a name="access-services-retirement"></a>Vyřazení služeb accessu

Jak jsme původně oznámili v mc97576, v březnu 2017 a během minulého roku jsme dál komunikovali, Access Services jsou vyřazeni. Další fází tohoto procesu bude odebrání webových databází Accessu, které používají SharePoint jako jejich podkladové úložiště dat.

**Jak to ovlivní mě?**

Od června 2019 zastavíme vytváření nových databází Accessu v SharePoint Online a do dubna 2020 vypneme službu a všechny zbývající aplikace.

**Co je potřeba udělat, abych se na tuto změnu připravil?**

Doporučujeme vám vytvořit plán přechodu pro webové databáze Accessu vaší organizace. Správci mohou pomocí [SharePoint aplikace pro Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) získat inventář aplikací pro Access, které weby používají.

Data webových databází Accessu můžete migrovat několika způsoby:

- Import do místní databáze Accessu (. ACCDB) nebo do Excel souboru.
- Doporučujeme také prozkoumat Microsoft PowerApps jako alternativní platformu pro vytváření firemních řešení bez kódu pro webová a mobilní zařízení.