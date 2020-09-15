---
title: Problémy s přihlášením k aplikacím Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695280"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="9a855-102">Prázdná přihlašovací obrazovka v aplikacích Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9a855-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="9a855-103">Tento problém můžete vyřešit takto:</span><span class="sxs-lookup"><span data-stu-id="9a855-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9a855-104">Nainstalujte si nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9a855-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9a855-105">Obnovení možností Internet Exploreru: přejděte na **nástroje**  >  **Možnosti Internetu**–  >  **Rozšířené**  >  **Obnovení nastavení Internet Exploreru** (Všimněte si, že ztratíte vlastní nastavení) a zkuste se znovu přihlásit k Office.</span><span class="sxs-lookup"><span data-stu-id="9a855-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9a855-106">Zakažte ochranu Application Guard v programu Windows Defender (WDAG) nebo podobný program brány firewall nebo antivirového programu:</span><span class="sxs-lookup"><span data-stu-id="9a855-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9a855-107">V Ovládacích panelech přejděte na **programy**a pak zvolte **zapnout nebo vypnout funkce systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="9a855-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9a855-108">Pokud je zapnutá ochrana Application Guard v programu Windows Defender, zkuste ho zakázat.</span><span class="sxs-lookup"><span data-stu-id="9a855-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9a855-109">**Poznámka:** Možná bude potřeba restartovat počítač.</span><span class="sxs-lookup"><span data-stu-id="9a855-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9a855-110">Ujistěte se, že [modul plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. aad. BrokerPlugin AAD není blokován žádnou aplikací ani bránou firewall/antivirový program.</span><span class="sxs-lookup"><span data-stu-id="9a855-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9a855-111">Pomocí Správce přihlašovacích údajů systému Windows [vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="9a855-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9a855-112">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16,0.</span><span class="sxs-lookup"><span data-stu-id="9a855-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9a855-113">(Např.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9a855-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9a855-114">Další informace najdete v článku [problémy s připojením při přihlášení po aktualizaci na Office 2016 Build 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9a855-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>