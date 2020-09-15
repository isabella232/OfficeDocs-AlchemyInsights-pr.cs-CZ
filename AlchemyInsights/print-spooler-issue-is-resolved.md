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
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="75109-102">Problém se zařazováním tisku je vyřešený</span><span class="sxs-lookup"><span data-stu-id="75109-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="75109-103">Pokud se vaše zařízení aktualizovalo na Windows 10  **OS Build 19041,329**, mohl se zaznamenat problém, kdy se určité tiskárny nedají vytisknout.</span><span class="sxs-lookup"><span data-stu-id="75109-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="75109-104">Služba zařazování tisku může při pokusu o tisk vyvolat chybu nebo ukončit neočekávané ukončení a žádný výstup nepochází z příslušné tiskárny.</span><span class="sxs-lookup"><span data-stu-id="75109-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="75109-105">Tento problém je vyřešený v buildu OS  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="75109-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="75109-106">**Průběžné šetření**</span><span class="sxs-lookup"><span data-stu-id="75109-106">**Ongoing investigation**</span></span>

<span data-ttu-id="75109-107">V některých zařízeních se může zdařit Chyba služby LSASS (Local Security Authority Subsystem Service) (**Isass.exe**) s chybovou zprávou "důležitý systémový proces, C:\WINDOWS\system32\Isass.exe, došlo k selhání kódu c0000008.</span><span class="sxs-lookup"><span data-stu-id="75109-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="75109-108">Počítač musí být restartován.</span><span class="sxs-lookup"><span data-stu-id="75109-108">The machine must now be restarted".</span></span>  <span data-ttu-id="75109-109">**Microsoft pracuje na řešení a poskytne aktualizaci v nadcházející verzi.**</span><span class="sxs-lookup"><span data-stu-id="75109-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="75109-110">Další informace najdete v informacích o  [známých problémech s Windows 10 verze 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="75109-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>