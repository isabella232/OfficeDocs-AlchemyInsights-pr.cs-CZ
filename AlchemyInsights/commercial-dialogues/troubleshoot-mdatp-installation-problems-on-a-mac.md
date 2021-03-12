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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744657"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="25493-102">Řešení problémů s instalací MDATP na Macu</span><span class="sxs-lookup"><span data-stu-id="25493-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="25493-103">Pokud ruční instalace selže, **zobrazí se na** stránce Souhrn v průvodci instalací tato chyba:</span><span class="sxs-lookup"><span data-stu-id="25493-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="25493-104">"Při instalaci došlo k chybě.</span><span class="sxs-lookup"><span data-stu-id="25493-104">"An error occurred during installation.</span></span> <span data-ttu-id="25493-105">Instalační program zjistil chybu, která způsoboval selhání instalace.</span><span class="sxs-lookup"><span data-stu-id="25493-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="25493-106">Požádejte o pomoc výrobce softwaru."</span><span class="sxs-lookup"><span data-stu-id="25493-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="25493-107">U nasazení MDM se na stránce zobrazuje i obecná chyba instalace.</span><span class="sxs-lookup"><span data-stu-id="25493-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="25493-108">I když se koncovým uživatelům nezobrazují přesné chyby, udržme soubor protokolu s průběhem instalace v **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="25493-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="25493-109">Každá instalační relace se připojí k tomuto souboru protokolu.</span><span class="sxs-lookup"><span data-stu-id="25493-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="25493-110">Pokud chcete vysílovat jenom poslední relaci instalace, použijte `sed` .</span><span class="sxs-lookup"><span data-stu-id="25493-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="25493-111">Další informace najdete v tématu Řešení potíží s [instalací pro microsoft defender atp pro Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="25493-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
