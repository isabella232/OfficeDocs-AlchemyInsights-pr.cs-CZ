---
title: Řešení problémů při instalaci Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002292"
- "4441"
ms.openlocfilehash: 4b309039dc920089d966e3bbe45dcea874668597
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695498"
---
# <a name="solutions-for-issues-when-installing-office"></a><span data-ttu-id="a997f-102">Řešení problémů při instalaci Office</span><span class="sxs-lookup"><span data-stu-id="a997f-102">Solutions for issues when installing Office</span></span>

<span data-ttu-id="a997f-103">Tady je několik řešení, pomocí kterých můžete zkusit odstranit chybu Office:</span><span class="sxs-lookup"><span data-stu-id="a997f-103">Try one of these solutions to fix your Office error:</span></span>

- <span data-ttu-id="a997f-104">Ujistěte se, že jste místním správcem počítače.</span><span class="sxs-lookup"><span data-stu-id="a997f-104">Ensure you are the local admin on the computer.</span></span> <span data-ttu-id="a997f-105">Restartujte počítač a zkuste [nainstalovat Office](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="a997f-105">Restart the computer and try [installing Office](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

- <span data-ttu-id="a997f-106">Na dotyčném počítači [zkontrolujte bránu firewall](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checkfirewall), [zkontrolujte antivirový software](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checkav) a [zkontrolujte nastavení proxy](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checkproxy).</span><span class="sxs-lookup"><span data-stu-id="a997f-106">[Check your firewall](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checkfirewall), [Check your antivirus software](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checkav), [Check your proxy settings](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380#bkmk_checkproxy) on the affected machine.</span></span>

- <span data-ttu-id="a997f-107">Odstraňte všechny předchozí stopy sady Office a k její přeinstalaci použijte nástroj Support and Recovery Assistant (SaRA).</span><span class="sxs-lookup"><span data-stu-id="a997f-107">Clean up any previous traces of Office and reinstall using the Support and Recovery Assistant (SaRA).</span></span> 

    - <span data-ttu-id="a997f-108">Stáhněte si nástroj [Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) a nainstalujte ho.</span><span class="sxs-lookup"><span data-stu-id="a997f-108">Download and install the [Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span> <span data-ttu-id="a997f-109">Až se otevře okno pro **odinstalaci produktů Office**, vyberte verzi, kterou chcete odinstalovat (pokud taková existuje), a klikněte na **Další**.</span><span class="sxs-lookup"><span data-stu-id="a997f-109">When it opens, from **Uninstall Office products** select the version you want to uninstall (if any) and click **Next**.</span></span> <span data-ttu-id="a997f-110">Pokračujte v procházení jednotlivých obrazovek a po zobrazení výzvy restartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="a997f-110">Continue going through screens and restart your computer when prompted.</span></span> <span data-ttu-id="a997f-111">Po restartování se nástroj SaRA automaticky znovu otevře pro dokončení procesu odinstalace.</span><span class="sxs-lookup"><span data-stu-id="a997f-111">After restarting, the SaRA automatically re-opens to complete the uninstall process.</span></span>
    - <span data-ttu-id="a997f-112">Použijte SaRA k [přeinstalaci Office](https://aka.ms/sara-officeinstall).</span><span class="sxs-lookup"><span data-stu-id="a997f-112">Use SaRA to [reinstall Office](https://aka.ms/sara-officeinstall).</span></span> <span data-ttu-id="a997f-113">**Poznámka:** Pokud chcete pomocí SaRA nastavit Visio nebo Project, použijte [instalaci Visia](https://aka.ms/SaRA-VisioSetupScenario) nebo [instalaci Projectu](https://aka.ms/SaRA-ProjectSetupScenario).</span><span class="sxs-lookup"><span data-stu-id="a997f-113">**Note**: For setting up Visio or Project using SaRA, use [Install Visio](https://aka.ms/SaRA-VisioSetupScenario) or [Install Project](https://aka.ms/SaRA-ProjectSetupScenario).</span></span>  

- <span data-ttu-id="a997f-114">K instalaci Office [použijte offline instalační program Office](https://support.office.com/article/f0a85fe7-118f-41cb-a791-d59cef96ad1c?wt.mc_id=Alchemy_ClientDIA).</span><span class="sxs-lookup"><span data-stu-id="a997f-114">[Use the Office offline installer](https://support.office.com/article/f0a85fe7-118f-41cb-a791-d59cef96ad1c?wt.mc_id=Alchemy_ClientDIA) to install Office.</span></span>

<span data-ttu-id="a997f-115">Řešení pro konkrétní kódy chyb při instalaci Office najdete v části **Chybové zprávy při instalaci Office** v tématu [Řešení potíží s instalací Office](https://support.office.com/article/35ff2def-e0b2-4dac-9784-4cf212c1f6c2#BKMK_ErrorMessages).</span><span class="sxs-lookup"><span data-stu-id="a997f-115">For solutions to specific Office installation error codes, see the **Error messages when installing Office** section in [Troubleshoot installing Office](https://support.office.com/article/35ff2def-e0b2-4dac-9784-4cf212c1f6c2#BKMK_ErrorMessages).</span></span>

