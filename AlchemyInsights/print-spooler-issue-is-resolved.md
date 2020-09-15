---
title: Problém se zařazováním tisku je vyřešený
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
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801834"
---
# <a name="print-spooler-issue-is-resolved"></a>Problém se zařazováním tisku je vyřešený

Pokud se vaše zařízení aktualizovalo na Windows 10  **OS Build 19041,329**, mohl se zaznamenat problém, kdy se určité tiskárny nedají vytisknout. Služba zařazování tisku může při pokusu o tisk vyvolat chybu nebo ukončit neočekávané ukončení a žádný výstup nepochází z příslušné tiskárny. Tento problém je vyřešený v buildu OS  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Průběžné šetření**

V některých zařízeních se může zdařit Chyba služby LSASS (Local Security Authority Subsystem Service) (**Isass.exe**) s chybovou zprávou "důležitý systémový proces, C:\WINDOWS\system32\Isass.exe, došlo k selhání kódu c0000008. Počítač musí být restartován.  **Microsoft pracuje na řešení a poskytne aktualizaci v nadcházející verzi.**

Další informace najdete v informacích o  [známých problémech s Windows 10 verze 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).