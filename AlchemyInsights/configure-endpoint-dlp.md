---
title: Konfigurovat ochranu před únikem informací pro koncové body
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402408"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="3c32a-102">Konfigurovat ochranu před únikem informací pro koncové body</span><span class="sxs-lookup"><span data-stu-id="3c32a-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="3c32a-103">Ochrana před únikem informací koncového bodu Microsoft umožňuje rozšířit možnosti ochrany před únikem informací a sledování citlivých informací na zařízeních s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3c32a-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="3c32a-104">Jakmile zařízení nahlásíte do správy zařízení, můžete vytvořit zásady ochrany před únikem informací, které budou vynucovat ochranná opatření pro položky.</span><span class="sxs-lookup"><span data-stu-id="3c32a-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="3c32a-105">Pomocí Průzkumníka aktivit můžete sledovat aktivitu citlivých položek.</span><span class="sxs-lookup"><span data-stu-id="3c32a-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="3c32a-106">Další informace najdete v článku [Onboarding zařízení do správy zařízení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="3c32a-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="3c32a-107">Jak začít používat ochranu před únikem informací koncového bodu:</span><span class="sxs-lookup"><span data-stu-id="3c32a-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="3c32a-108">Ujistěte se, že máte odpovídající licence skladové jednotky (SKU) nebo předplatného.</span><span class="sxs-lookup"><span data-stu-id="3c32a-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="3c32a-109">Další informace najdete v článku [Licence SKU nebo předplatného](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="3c32a-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="3c32a-110">Zkontrolujte oprávnění potřebná k povolení správy zařízení, přístupu na stránku pro onboarding nebo zapnutí/vypnutí monitorování zařízení.</span><span class="sxs-lookup"><span data-stu-id="3c32a-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="3c32a-111">Další informace najdete v článku na téma [Oprávnění](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="3c32a-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="3c32a-112">Zařízení můžete zapojit do Správy zařízení, když budete postupovat podle návodu na onboarding nového zařízení.</span><span class="sxs-lookup"><span data-stu-id="3c32a-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="3c32a-113">Pokud v části Dodržování předpisů M365 **Nastavení** chybí možnost Onboarding zařízení (náhled), zkontrolujte, jestli máte odpovídající licenci a oprávnění, na které se odkazuje výše.</span><span class="sxs-lookup"><span data-stu-id="3c32a-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="3c32a-114">Další informace najdete v článku [Onboarding zařízení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="3c32a-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="3c32a-115">Vytvořte zásady ochrany před únikem informací, které ochrání vaše citlivé položky.</span><span class="sxs-lookup"><span data-stu-id="3c32a-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="3c32a-116">Informace najdete v článku [Scénáře zásad ochrany před únikem informací koncových bodů](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="3c32a-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="3c32a-117">Další informace o ochraně před únikem informací pro koncové body Microsoftu najdete v článku [Ochrana před únikem informací koncových bodů Microsoftu 365 (náhled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="3c32a-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="3c32a-118">**Postup při Shromažďování důležitých dat, pokud je potřeba podpora:**</span><span class="sxs-lookup"><span data-stu-id="3c32a-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="3c32a-119">Stáhněte si MDATP Client Analyzer ve verzi Preview z [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="3c32a-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="3c32a-120">V okně cmd spusťte nástroj jako správce:</span><span class="sxs-lookup"><span data-stu-id="3c32a-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="3c32a-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="3c32a-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="3c32a-122">Po zobrazení výzvy „Zadejte počet minut potřebných ke shromáždění dat sledování:“, zadejte počet minut, které jsou potřeba k provedení scénáře.</span><span class="sxs-lookup"><span data-stu-id="3c32a-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="3c32a-123">Spustit scénář</span><span class="sxs-lookup"><span data-stu-id="3c32a-123">Run the scenario</span></span>

<span data-ttu-id="3c32a-124">Získaný výstup souboru ZIP se předá agentovi podpory.</span><span class="sxs-lookup"><span data-stu-id="3c32a-124">Collect the Zip file output to be given to the Support agent.</span></span>
