---
title: Inventář zařízení Intune
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
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014065"
---
# <a name="intune-device-inventory"></a>Inventář zařízení Intune

Okno Zařízení poskytuje správci přehled o zařízeních spravovaných v Intune na základě zařízení. Zobrazené informace zahrnují: Hardware, Zjištěné aplikace, Stav dodržování předpisů zařízení a Stav konfigurace zařízení.

Data inventáře hardwaru a zjištěných aplikací se shromažďují v sedmidenním cyklu. Aplikace a konkrétní prvky oznámené hardwaru se liší v závislosti na operačním systému zařízení a na tom, jestli je zařízení vlastněné osobně nebo firemním vlastnictvím.

Další informace najdete v tématu [Zobrazení podrobností o zařízení v Intune](https://docs.microsoft.com/intune/device-inventory).

**Nejčastější dotazy**

Otázka: Nepřijímám úplný inventář aplikací, které jsou na zařízeních zaregistrované Windows Intune.Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices. Proč ne?

O: V současné době jsou uvedené jenom moderní aplikace pro Windows 10 počítačů, které jsou identifikované jako podniková zařízení. Intune neshromažďuje informace o aplikacích Win32 nainstalovaných na těchto zařízeních.

Otázka: Proč nejsou telefonní čísla shromažďována ze všech zařízení?

O: Telefony zařazené do kategorií jako podniková zařízení v Intune se při spuštění sestavy inventáře mobilních zařízení ne identifikují s jejich celým telefonním číslem. Telefonní čísla s vlastním zařízením jsou vždy částečně maskovaná hvězdičkami (****) a zobrazují se jenom poslední čtyři číslice.