---
title: Řešení problémů s instalací MDATP na Macu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693350"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="22e27-102">Řešení problémů s instalací MDATP na Macu</span><span class="sxs-lookup"><span data-stu-id="22e27-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="22e27-103">Pokud se ruční instalace **nezdaří,** zobrazí se na stránce Souhrn v Průvodci instalací tato chybová zpráva:</span><span class="sxs-lookup"><span data-stu-id="22e27-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="22e27-104">"Při instalaci došlo k chybě.</span><span class="sxs-lookup"><span data-stu-id="22e27-104">"An error occurred during installation.</span></span> <span data-ttu-id="22e27-105">Instalační program narazil na chybu, která způsoboval selhání instalace.</span><span class="sxs-lookup"><span data-stu-id="22e27-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="22e27-106">Požádejte o pomoc výrobce softwaru."</span><span class="sxs-lookup"><span data-stu-id="22e27-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="22e27-107">U nasazení MDM se na stránce zobrazuje také obecná chyba instalace.</span><span class="sxs-lookup"><span data-stu-id="22e27-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="22e27-108">Ačkoli koncovým uživatelům nezobrazujíme přesné chyby, uchováme soubor protokolu s průběhem instalace v **umístění /Library/Logs/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="22e27-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="22e27-109">Každá instalační relace se připojí k tomuto souboru protokolu.</span><span class="sxs-lookup"><span data-stu-id="22e27-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="22e27-110">Pokud chcete výstupovat jenom poslední relaci instalace, použijte `sed` .</span><span class="sxs-lookup"><span data-stu-id="22e27-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="22e27-111">Další informace najdete v článku Řešení potíží s [instalací nástroje Microsoft Defender ATP pro Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="22e27-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
