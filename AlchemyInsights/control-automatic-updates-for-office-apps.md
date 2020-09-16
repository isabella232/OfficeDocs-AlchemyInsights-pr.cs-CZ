---
title: Řízení automatických aktualizací pro aplikace Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747769"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="6789f-102">Řízení automatických aktualizací pro aplikace Office</span><span class="sxs-lookup"><span data-stu-id="6789f-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="6789f-103">Ve výchozím nastavení se aktualizace aplikací Office automaticky stáhnou a použijí se na pozadí bez zásahu uživatele.</span><span class="sxs-lookup"><span data-stu-id="6789f-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="6789f-104">Správci ale můžou řídit, jak se aktualizace používají pomocí nastavení Office Update.</span><span class="sxs-lookup"><span data-stu-id="6789f-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="6789f-105">Nastavení aktualizací: umožňuje správcům povolit nebo zakázat automatické aktualizace, zobrazit nebo skrýt v Office tlačítko **aktualizovat** , nastavit termíny aktualizace a další.</span><span class="sxs-lookup"><span data-stu-id="6789f-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="6789f-106">Podrobné informace najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="6789f-106">For detailed information, see:</span></span>

- [<span data-ttu-id="6789f-107">Konfigurace nastavení aktualizací pro Office</span><span class="sxs-lookup"><span data-stu-id="6789f-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="6789f-108">Automatická aktualizace Office není povolená.</span><span class="sxs-lookup"><span data-stu-id="6789f-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="6789f-109">Určení způsobu aktualizace Office po instalaci</span><span class="sxs-lookup"><span data-stu-id="6789f-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="6789f-110">Pokud chcete zkontrolovat nastavení existujících aktualizací použitých pro klientský počítač, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="6789f-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="6789f-111">Otevřete Editor registru **– Spusťte nástroj**  >  **Run**  >  **Regedit**.</span><span class="sxs-lookup"><span data-stu-id="6789f-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="6789f-112">Přejděte do následujícího umístění a zkontrolujte nastavení aktualizace Office:</span><span class="sxs-lookup"><span data-stu-id="6789f-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="6789f-113">a.</span><span class="sxs-lookup"><span data-stu-id="6789f-113">a.</span></span> <span data-ttu-id="6789f-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="6789f-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="6789f-115">b.</span><span class="sxs-lookup"><span data-stu-id="6789f-115">b.</span></span> <span data-ttu-id="6789f-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="6789f-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="6789f-117">**Poznámka:**  Pokud je nastaven klíč OfficeMgmtCOM, může se zobrazit zpráva "aktualizace jsou spravovány správcem systému **" v**  >  **Account**  >  **aktualizacích Office Account Updates**.</span><span class="sxs-lookup"><span data-stu-id="6789f-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="6789f-118">Další informace najdete v článku [Správa aktualizací aplikací microsoft 365 pomocí nástroje Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="6789f-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  