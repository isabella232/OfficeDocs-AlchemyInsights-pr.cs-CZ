---
title: Byl vyřešen problém se zařazovacími službami tisku.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088303"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="24e95-102">Byl vyřešen problém se zařazovacími službami tisku.</span><span class="sxs-lookup"><span data-stu-id="24e95-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="24e95-103">Pokud bylo vaše zařízení aktualizováno systémem Windows 10 **OS Build 19041.329**, možná jste zaznamenali problém, kdy některé tiskárny netiskly.</span><span class="sxs-lookup"><span data-stu-id="24e95-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="24e95-104">Zařazování tisku může vyvolat chybu nebo neočekávaně zavřít při pokusu o tisk a žádný výstup pochází z postižené tiskárny.</span><span class="sxs-lookup"><span data-stu-id="24e95-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="24e95-105">Tento problém je vyřešen v sestavení operačního systému **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="24e95-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="24e95-106">**Probíhající šetření**</span><span class="sxs-lookup"><span data-stu-id="24e95-106">**Ongoing investigation**</span></span>

<span data-ttu-id="24e95-107">Soubor LSASS**Isass.exe**(LSASS) místního úřadu zabezpečení může na některých zařízeních selhat s chybovou zprávou "Kritický systémový proces C:\WINDOWS\system32\Isass.exe se stavovým kódem c0000008 selhal.</span><span class="sxs-lookup"><span data-stu-id="24e95-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="24e95-108">Zařízení musí být nyní restartováno".</span><span class="sxs-lookup"><span data-stu-id="24e95-108">The machine must now be restarted".</span></span>  <span data-ttu-id="24e95-109">**Společnost Microsoft pracuje na řešení a poskytne aktualizaci v nadcházející verzi.**</span><span class="sxs-lookup"><span data-stu-id="24e95-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="24e95-110">Další informace naleznete ve [známých problémech se systémem Windows 10 Verze 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="24e95-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>