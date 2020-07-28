---
title: Řízení automatických aktualizací pro aplikace Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438839"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="40bb0-102">Řízení automatických aktualizací pro aplikace Office</span><span class="sxs-lookup"><span data-stu-id="40bb0-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="40bb0-103">Ve výchozím nastavení se aktualizace aplikací Office stahují automaticky a aplikují se na pozadí bez zásahu uživatele.</span><span class="sxs-lookup"><span data-stu-id="40bb0-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="40bb0-104">Správci však mohou řídit způsob použití aktualizací pomocí nastavení služby Office Update.</span><span class="sxs-lookup"><span data-stu-id="40bb0-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="40bb0-105">Nastavení aktualizací umožňuje správcům povolit nebo zakázat automatické aktualizace, zobrazit nebo skrýt tlačítko **Aktualizovat** v Office, nastavit termíny aktualizace a další.</span><span class="sxs-lookup"><span data-stu-id="40bb0-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="40bb0-106">Podrobné informace naleznete v tématu:</span><span class="sxs-lookup"><span data-stu-id="40bb0-106">For detailed information, see:</span></span>

- [<span data-ttu-id="40bb0-107">Konfigurace nastavení aktualizací pro Office</span><span class="sxs-lookup"><span data-stu-id="40bb0-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="40bb0-108">Automatické aktualizace pro Office nejsou povoleny.</span><span class="sxs-lookup"><span data-stu-id="40bb0-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="40bb0-109">Definování způsobu aktualizace Office po instalaci</span><span class="sxs-lookup"><span data-stu-id="40bb0-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="40bb0-110">Chcete-li zkontrolovat existující nastavení aktualizací použitá pro klientský počítač, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="40bb0-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="40bb0-111">Otevřete Editor registru tak, že přejdete na **spustit**  >  **Run**  >  **spustit regedit**.</span><span class="sxs-lookup"><span data-stu-id="40bb0-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="40bb0-112">Přepněte do následujícího umístění a zkontrolujte nastavení Office Update:</span><span class="sxs-lookup"><span data-stu-id="40bb0-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="40bb0-113">a.</span><span class="sxs-lookup"><span data-stu-id="40bb0-113">a.</span></span> <span data-ttu-id="40bb0-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="40bb0-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="40bb0-115">b.</span><span class="sxs-lookup"><span data-stu-id="40bb0-115">b.</span></span> <span data-ttu-id="40bb0-116">ClickToRun\Konfigurace</span><span class="sxs-lookup"><span data-stu-id="40bb0-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="40bb0-117">**Poznámka:**  Pokud je klíč OfficeMgmtCOM nastavený, může se v **Office**  >  **aktualizacích sady**Office Office zobrazit zpráva "Aktualizace jsou spravovány správcem systému"  >  **Office Updates**.</span><span class="sxs-lookup"><span data-stu-id="40bb0-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="40bb0-118">Další informace najdete v [tématu Správa aktualizací aplikací Microsoft 365 pomocí Nástroje pro konfiguračního bodu Microsoft.](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)</span><span class="sxs-lookup"><span data-stu-id="40bb0-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  