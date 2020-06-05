---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579894"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="09529-102">Prázdná přihlašovací obrazovka v aplikacích Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="09529-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="09529-103">Chcete-li tento problém vyřešit, vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="09529-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="09529-104">Nainstalujte nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="09529-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="09529-105">Obnovení možností aplikace Internet Explorer: Přejděte na **Nástroje**  >  **k**  >  **Advanced**  >  **rozšířenému obnovení nastavení aplikace Internet Explorer** (nezapomeňte, že ztratíte vlastní nastavení), a zkuste se znovu přihlásit k Office.</span><span class="sxs-lookup"><span data-stu-id="09529-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="09529-106">Zakažte ochranu aplikací programu Windows Defender (WDAG) nebo podobný firewall nebo antivirový program:</span><span class="sxs-lookup"><span data-stu-id="09529-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="09529-107">V Ovládacích panelech přejděte na **Programy**a pak zvolte **Zapnout nebo vypnout funkce systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="09529-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="09529-108">Pokud je zapnutý program Ochrana aplikací programu Windows Defender, zkuste jej zakázat.</span><span class="sxs-lookup"><span data-stu-id="09529-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="09529-109">**Poznámka:** Pravděpodobně bude nutné restartovat počítač.</span><span class="sxs-lookup"><span data-stu-id="09529-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="09529-110">Ujistěte se, že modul plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) není blokován žádnou aplikací nebo bránou firewall/antivirovým programem.</span><span class="sxs-lookup"><span data-stu-id="09529-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="09529-111">[Vymazání přihlašovacích údajů Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce pověření systému Windows</span><span class="sxs-lookup"><span data-stu-id="09529-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="09529-112">**Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0.</span><span class="sxs-lookup"><span data-stu-id="09529-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="09529-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="09529-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="09529-114">Další informace najdete [v tématu Problémy s připojením při přihlášení po aktualizaci na sestavení Office 2016 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="09529-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>