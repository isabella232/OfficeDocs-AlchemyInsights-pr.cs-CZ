---
title: Intune – inventář zařízení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667871"
---
# <a name="intune-device-inventory"></a>Intune – inventář zařízení

Okno zařízení poskytuje správci přehled o zařízeních ve správě v Intune na jednotlivých zařízeních. Zobrazené informace zahrnují: hardware, zjištěné aplikace, stav shody zařízení a stav konfigurace zařízení.

Data inventáře pro hardware a zjištěné aplikace se shromažďují po sedmi dnech. Uvedené aplikace a zvláštní prvky hardwaru se liší v závislosti na operačním systému zařízení a na tom, jestli je dané zařízení osobně nebo podnikově vlastněné.

Další informace najdete v tématu [zobrazení podrobností o zařízení v Intune](https://docs.microsoft.com/intune/device-inventory).

**Nejčastější dotazy**

Otázka: mi se nezobrazuje seznam úplný soupis aplikací v Intune – registrovaná zařízení s Windows. Proč ne?

A: pro počítače s Windows 10, které jsou označené jako podniková zařízení, jsou v současnosti uvedené jenom moderní aplikace. Intune neshromažďuje informace o aplikacích Win32 nainstalovaných na těchto zařízeních.

Otázka: Proč se telefonní čísla neshromažďují ze všech zařízení?

A: telefony, které jsou v Intune zařazené do kategorií, se neidentifikují s plným telefonním číslem, když třeba spustíte sestavu inventáře mobilních zařízení. Osobní telefonní čísla zařízení jsou vždy částečně maskována pomocí hvězdiček (* * * *) a zobrazují jenom poslední čtyři číslice.