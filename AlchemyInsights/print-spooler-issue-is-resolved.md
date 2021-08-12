---
title: Problém se zařazováním tisku je vyřešený.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911331"
---
# <a name="print-spooler-issue-is-resolved"></a>Problém se zařazováním tisku je vyřešený.

Pokud se vaše zařízení aktualizovalo buildem  **19041.329** operačního systému Windows 10, mohli jste pozorovat problém, kdy se některé tiskárny nepodařilo vytisknout. Služba zařazování tisku může při pokusu o tisk vyvolat chybu nebo se neočekávaně zavřít a z ovlivněné tiskárny není žádný výstup. Tento problém je vyřešený v buildu operačního systému  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Probíhající vyšetřování**

Soubor lsass (Local Security Authority Subsystem Service)**(Isass.exe)** se může na některých zařízeních s chybovou zprávou "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008" (Kritický systémový proces, C:\WINDOWS\system32\Isass.exe) se nezdařil s kódem stavu c0000008. Počítač teď musí být restartován".  **Microsoft pracuje na řešení a poskytne aktualizaci v nadcházející verzi.**

Další informace najdete ve  [Windows 10 verze 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)– známé problémy .