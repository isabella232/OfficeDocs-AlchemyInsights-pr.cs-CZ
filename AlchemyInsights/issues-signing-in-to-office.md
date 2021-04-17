---
title: Problémy s přihlášením k aplikacím Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833024"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="afbdb-102">Prázdná přihlašovací obrazovka v aplikacích Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="afbdb-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="afbdb-103">Pokud chcete tento problém vyřešit, zkuste následující postup:</span><span class="sxs-lookup"><span data-stu-id="afbdb-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="afbdb-104">Nainstalujte si nejnovější aktualizace [pro Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="afbdb-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="afbdb-105">Resetovat možnosti Internet Exploreru: Přejděte na Nástroje Možnosti internetu Upřesnit resetování nastavení  >    >    >  **Internet Exploreru** (všimněte si, že přijdete o vlastní nastavení) a zkuste se přihlásit k Office znovu.</span><span class="sxs-lookup"><span data-stu-id="afbdb-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="afbdb-106">Zakažte Ochranu aplikací v programu Windows Defender (WDAG) nebo podobný firewall nebo antivirový program:</span><span class="sxs-lookup"><span data-stu-id="afbdb-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="afbdb-107">V Ovládacích panelech přejděte na **Programy** a pak zvolte **Zapnout nebo vypnout** funkce Windows.</span><span class="sxs-lookup"><span data-stu-id="afbdb-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="afbdb-108">Pokud je povolená ochrana Application Guard v programu Windows Defender, zkuste ji zakázat.</span><span class="sxs-lookup"><span data-stu-id="afbdb-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="afbdb-109">**Poznámka:** Možná budete muset restartovat počítač.</span><span class="sxs-lookup"><span data-stu-id="afbdb-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="afbdb-110">Ujistěte se, že modul plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) není blokován žádnou aplikací nebo bránou firewall nebo antivirovým programem.</span><span class="sxs-lookup"><span data-stu-id="afbdb-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="afbdb-111">[Vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce přihlašovacích údajů systému Windows.</span><span class="sxs-lookup"><span data-stu-id="afbdb-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="afbdb-112">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0.</span><span class="sxs-lookup"><span data-stu-id="afbdb-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="afbdb-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="afbdb-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="afbdb-114">Další informace najdete v článku Problémy s připojením při přihlašování po aktualizaci na [build 16.0.7967 Office 2016 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="afbdb-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>