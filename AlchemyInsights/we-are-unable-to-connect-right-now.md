---
title: Problém s aktivací – nyní se nemůžeme připojit.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581868"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="1a8a0-102">Oprava zprávy Aplikace Microsoft 365 "Nejsme schopni se připojit právě teď"</span><span class="sxs-lookup"><span data-stu-id="1a8a0-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="1a8a0-103">Pokud se zobrazí tato zpráva, vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="1a8a0-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="1a8a0-104">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, zda neblokují přístup k Internetu aplikacím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1a8a0-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="1a8a0-105">Viz [Microsoft URL a IP adresy rozsahy](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="1a8a0-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="1a8a0-106">Přejděte na **spustit**  >  **Run**a zadejte **soubor services.msc**.</span><span class="sxs-lookup"><span data-stu-id="1a8a0-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="1a8a0-107">Ujistěte se, že jsou spuštěny všechny následující služby:</span><span class="sxs-lookup"><span data-stu-id="1a8a0-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="1a8a0-108">Automatické nastavení síťových připojených zařízení</span><span class="sxs-lookup"><span data-stu-id="1a8a0-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="1a8a0-109">Služba seznamu sítí</span><span class="sxs-lookup"><span data-stu-id="1a8a0-109">Network List Service</span></span>
    - <span data-ttu-id="1a8a0-110">Povědomí o poloze v síti</span><span class="sxs-lookup"><span data-stu-id="1a8a0-110">Network Location Awareness</span></span>
    - <span data-ttu-id="1a8a0-111">Protokol událostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="1a8a0-111">Windows Event Log</span></span>

<span data-ttu-id="1a8a0-112">Pokud není spuštěna jedna z těchto služeb, zkuste ji spustit.</span><span class="sxs-lookup"><span data-stu-id="1a8a0-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="1a8a0-113">Pokud máte potíže se spuštěním služby, spusťte následující příkaz otevřením příkazového řádku se zvýšenými oprávněními:</span><span class="sxs-lookup"><span data-stu-id="1a8a0-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="1a8a0-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="1a8a0-114">**sfc /scannow**</span></span>

<span data-ttu-id="1a8a0-115">Po dokončení tohoto příkazu restartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="1a8a0-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="1a8a0-116">Podrobné informace naleznete v [tématu "Omlouváme se, ale nemůžeme se připojit k vašemu účtu. Opakujte akci později při aktivaci Office z Microsoftu 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="1a8a0-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>