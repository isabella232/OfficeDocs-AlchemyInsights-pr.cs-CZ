---
title: Problém s aktivací – teď se nemůžeme připojit
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725976"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="6e184-102">Oprava aplikací Microsoft 365 se nemůžete připojit hned "</span><span class="sxs-lookup"><span data-stu-id="6e184-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="6e184-103">Pokud se zobrazí tato zpráva, zkuste toto:</span><span class="sxs-lookup"><span data-stu-id="6e184-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6e184-104">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že nejsou blokovány internetové připojení k aplikacím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6e184-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="6e184-105">Viz [adresy URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6e184-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="6e184-106">Přejděte na **Spustit**  >  **Run**a zadejte **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="6e184-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="6e184-107">Zkontrolujte, jestli jsou všechny tyto služby běžící:</span><span class="sxs-lookup"><span data-stu-id="6e184-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="6e184-108">Automatická instalace zařízení připojeného k síti</span><span class="sxs-lookup"><span data-stu-id="6e184-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="6e184-109">Služba seznam sítě</span><span class="sxs-lookup"><span data-stu-id="6e184-109">Network List Service</span></span>
    - <span data-ttu-id="6e184-110">Povědomí o umístění v síti</span><span class="sxs-lookup"><span data-stu-id="6e184-110">Network Location Awareness</span></span>
    - <span data-ttu-id="6e184-111">Protokol událostí systému Windows</span><span class="sxs-lookup"><span data-stu-id="6e184-111">Windows Event Log</span></span>

<span data-ttu-id="6e184-112">Pokud není některá z těchto služeb spuštěná, zkuste ji spustit.</span><span class="sxs-lookup"><span data-stu-id="6e184-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="6e184-113">Pokud máte problém se spuštěním služby, spusťte příkazový řádek se zvýšenými oprávněními a spusťte následující příkaz:</span><span class="sxs-lookup"><span data-stu-id="6e184-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="6e184-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="6e184-114">**sfc /scannow**</span></span>

<span data-ttu-id="6e184-115">Po dokončení tohoto příkazu restartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="6e184-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="6e184-116">Podrobné informace najdete v [části "litujeme, ale nemůžeme se připojit ke svému účtu. Při aktivaci Office ze systému Microsoft 365 zkuste to znovu později](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="6e184-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>