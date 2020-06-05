---
title: Oprava aplikací Microsoft 365 Omlouváme se, máme zprávu o dočasných problémech se serverem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582696"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="fe026-102">Oprava zprávy Aplikace Microsoft 365 "Omlouváme se, máme problémy s dočasným serverem"</span><span class="sxs-lookup"><span data-stu-id="fe026-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="fe026-103">Pokud se zobrazí tato zpráva, vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="fe026-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fe026-104">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, zda neblokují přístup k Internetu aplikacím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fe026-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="fe026-105">Viz [adresy URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fe026-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fe026-106">Přejděte na **spustit**  >  **Run**a zadejte **soubor services.msc**.</span><span class="sxs-lookup"><span data-stu-id="fe026-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fe026-107">Ujistěte se, že jsou spuštěny všechny následující služby:</span><span class="sxs-lookup"><span data-stu-id="fe026-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fe026-108">Automatické nastavení síťových připojených zařízení</span><span class="sxs-lookup"><span data-stu-id="fe026-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fe026-109">Služba seznamu sítí</span><span class="sxs-lookup"><span data-stu-id="fe026-109">Network List Service</span></span>
    - <span data-ttu-id="fe026-110">Povědomí o poloze v síti</span><span class="sxs-lookup"><span data-stu-id="fe026-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fe026-111">Protokol událostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="fe026-111">Windows Event Log</span></span>

<span data-ttu-id="fe026-112">Pokud není spuštěna jedna z těchto služeb, zkuste ji spustit.</span><span class="sxs-lookup"><span data-stu-id="fe026-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fe026-113">Pokud máte potíže se spuštěním služby, spusťte následující příkaz otevřením příkazového řádku se zvýšenými oprávněními:</span><span class="sxs-lookup"><span data-stu-id="fe026-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fe026-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="fe026-114">**sfc /scannow**</span></span>

<span data-ttu-id="fe026-115">Po dokončení tohoto příkazu restartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="fe026-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fe026-116">Podrobné informace naleznete v [tématu "Omlouváme se, ale nemůžeme se připojit k vašemu účtu. Opakujte akci později" při aktivaci](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="fe026-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>