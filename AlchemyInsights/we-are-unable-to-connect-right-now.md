---
title: Problém s aktivací – teď se nemůžeme připojit
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806435"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="37e0d-102">Oprava zprávy o řešení aplikací Microsoft 365 "Právě se nemůžeme připojit".</span><span class="sxs-lookup"><span data-stu-id="37e0d-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="37e0d-103">Pokud se vám tato zpráva zobrazí, zkuste toto:</span><span class="sxs-lookup"><span data-stu-id="37e0d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="37e0d-104">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že neblokují přístup k internetu k aplikacím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="37e0d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="37e0d-105">Další informace najdete v článku Adresy URL a [rozsahy IP adres společnosti Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="37e0d-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="37e0d-106">Přejděte na **Spustit** spustit a  >  zadejte **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="37e0d-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="37e0d-107">Ujistěte se, že jsou všechny spuštěné následující služby:</span><span class="sxs-lookup"><span data-stu-id="37e0d-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="37e0d-108">Automatické nastavení zařízení připojených k síti</span><span class="sxs-lookup"><span data-stu-id="37e0d-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="37e0d-109">Network List Service</span><span class="sxs-lookup"><span data-stu-id="37e0d-109">Network List Service</span></span>
    - <span data-ttu-id="37e0d-110">Povědomí o umístění v síti</span><span class="sxs-lookup"><span data-stu-id="37e0d-110">Network Location Awareness</span></span>
    - <span data-ttu-id="37e0d-111">Protokol událostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="37e0d-111">Windows Event Log</span></span>

<span data-ttu-id="37e0d-112">Pokud jedna z těchto služeb není spuštěná, zkuste ji spustit.</span><span class="sxs-lookup"><span data-stu-id="37e0d-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="37e0d-113">Pokud máte potíže se spuštěním služby, spusťte následující příkaz tak, že otevřete příkazový řádek se zvýšenými oprávněními:</span><span class="sxs-lookup"><span data-stu-id="37e0d-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="37e0d-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="37e0d-114">**sfc /scannow**</span></span>

<span data-ttu-id="37e0d-115">Po dokončení tohoto příkazu restartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="37e0d-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="37e0d-116">Podrobné informace najdete v tématu [Omlouváme se, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později" při aktivaci Office z Microsoftu 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="37e0d-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>