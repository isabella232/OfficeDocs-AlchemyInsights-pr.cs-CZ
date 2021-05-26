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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657922"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="f8d8f-102">Konfigurovat ochranu před únikem informací pro koncové body</span><span class="sxs-lookup"><span data-stu-id="f8d8f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="f8d8f-103">Ochrana před únikem informací koncového bodu Microsoft umožňuje rozšířit možnosti ochrany před únikem informací a sledování citlivých informací na zařízeních s Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="f8d8f-104">Jakmile zařízení nahlásíte do správy zařízení, můžete vytvořit zásady ochrany před únikem informací, které budou vynucovat ochranná opatření pro položky.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="f8d8f-105">Pomocí Průzkumníka aktivit můžete sledovat aktivitu citlivých položek.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="f8d8f-106">Další informace najdete v článku [Onboarding zařízení do správy zařízení](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="f8d8f-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="f8d8f-107">Jak začít používat ochranu před únikem informací koncového bodu:</span><span class="sxs-lookup"><span data-stu-id="f8d8f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="f8d8f-108">Ujistěte se, že máte odpovídající licence skladové jednotky (SKU) nebo předplatného.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="f8d8f-109">Další informace najdete v článku [Licence SKU nebo předplatného](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="f8d8f-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="f8d8f-110">Zkontrolujte oprávnění potřebná k povolení správy zařízení, přístupu na stránku pro onboarding nebo zapnutí/vypnutí monitorování zařízení.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="f8d8f-111">Další informace najdete v článku na téma [Oprávnění](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="f8d8f-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="f8d8f-112">Zařízení můžete zapojit do Správy zařízení, když budete postupovat podle návodu na onboarding nového zařízení.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="f8d8f-113">Další informace najdete v článku [Onboarding zařízení](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="f8d8f-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="f8d8f-114">Vytvořte zásady ochrany před únikem informací, které ochrání vaše citlivé položky.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="f8d8f-115">Informace najdete v článku [Scénáře zásad ochrany před únikem informací koncových bodů](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="f8d8f-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="f8d8f-116">Další informace o ochraně před únikem informací pro koncové body Microsoftu najdete v článku [Ochrana před únikem informací koncových bodů Microsoftu 365 (náhled)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="f8d8f-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="f8d8f-117">**Postup při Shromažďování důležitých dat, pokud je potřeba podpora:**</span><span class="sxs-lookup"><span data-stu-id="f8d8f-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="f8d8f-118">Stáhněte [si MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="f8d8f-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="f8d8f-119">V okně cmd spusťte nástroj jako správce:</span><span class="sxs-lookup"><span data-stu-id="f8d8f-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="f8d8f-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="f8d8f-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="f8d8f-121">Po zobrazení výzvy zadejte počet minut ke shromažďování **trasování:**, zadejte počet minut nutný ke spuštění scénáře.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="f8d8f-122">Spusťte scénář.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-122">Run the scenario.</span></span>

<span data-ttu-id="f8d8f-123">Shromažďte výstup souboru ZIP, který chcete dát agentovi podpory.</span><span class="sxs-lookup"><span data-stu-id="f8d8f-123">Collect the Zip file output to give to the Support agent.</span></span>
