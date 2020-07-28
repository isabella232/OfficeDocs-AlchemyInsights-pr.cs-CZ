---
title: Inventář zařízení Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439161"
---
# <a name="intune-device-inventory"></a>Inventář zařízení Intune

Okno Zařízení poskytuje správci přehled o zařízeních, která jsou v rámci správy v Intune, a to na základě pro všechna zařízení. Zobrazené informace zahrnují: Hardware, Zjištěné aplikace, Stav kompatibility zařízení a stav konfigurace zařízení.

Data inventáře pro hardware a zjištěné aplikace jsou shromažďována v sedmidenním cyklu. Aplikace a konkrétní prvky hardwaru hlášené se liší v závislosti na operačním systému zařízení a zda je zařízení v osobním nebo vlastněném podniku.

Další informace najdete [v tématu Podrobnosti o zařízení v Intune](https://docs.microsoft.com/intune/device-inventory).

**Nejčastější dotazy**

Otázka: Nedostávám úplný soupis aplikací, které se na zařízeních s Windows zaregistrované v Intune nacházejí. Proč ne?

A: V současné době jsou uvedeny pouze moderní aplikace pro počítače s Windows 10, které jsou označeny jako podniková zařízení. Intune neshromažďuje informace o aplikacích Win32 nainstalovaných na těchto zařízeních.

Otázka: Proč nejsou telefonní čísla shromažďována ze všech zařízení?

A: Telefony zařazené do kategorie podnikových zařízení v Intune nejsou identifikovány s jejich úplným telefonním číslem, když například spustíte přehled inventáře mobilních zařízení. Telefonní čísla bring-you-own-device jsou vždy částečně maskována hvězdičkami (****) a zobrazují pouze poslední čtyři číslice.