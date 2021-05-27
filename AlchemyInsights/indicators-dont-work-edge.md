---
title: Indikátory nefungují v prohlížeči Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676131"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="b2493-102">Indikátory nefungují v prohlížeči Edge</span><span class="sxs-lookup"><span data-stu-id="b2493-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="b2493-103">Po vytvoření indikátoru ho Edge (Smartscreen) nebude ctít.</span><span class="sxs-lookup"><span data-stu-id="b2493-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="b2493-104">Další informace najdete v tématu Vytvoření indikátorů pro IP adresy a [adresy URL/domény](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="b2493-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="b2493-105">Krok 1: Zkontrolujte následující:</span><span class="sxs-lookup"><span data-stu-id="b2493-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="b2493-106">Ověřte, jestli je indikátor správný (žádné překlepy v IP/URL, správná akce, správné skupiny RBAC).</span><span class="sxs-lookup"><span data-stu-id="b2493-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="b2493-107">Počkejte minimálně 2 hodiny po vytvoření indikátoru, aby se zohlednila jakákoli možná latence.</span><span class="sxs-lookup"><span data-stu-id="b2493-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="b2493-108">Ujistěte se, že jsou systém(y) v programu Microsoft Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="b2493-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="b2493-109">Ověřte, jestli systém(y) může komunikovat s cloudem.</span><span class="sxs-lookup"><span data-stu-id="b2493-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="b2493-110">Ověřte, jestli je smartscreen povolený a dostupný, a to tak, že se dostanete na [testovací web.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="b2493-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="b2493-111">Krok 2: Řešení potenciálního problému</span><span class="sxs-lookup"><span data-stu-id="b2493-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="b2493-112">Ujistěte se, že klient splňuje požadavky.</span><span class="sxs-lookup"><span data-stu-id="b2493-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="b2493-113">Podrobnosti najdete v tématu Vytvoření indikátorů pro IP adresy a [adresy URL/domény](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="b2493-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="b2493-114">Ujistěte se, že používáte nejnovější verzi prohlížeče Edge.</span><span class="sxs-lookup"><span data-stu-id="b2493-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="b2493-115">Informace o nejnovější verzi najdete v tématu Zjistěte, kterou [Microsoft Edge máte](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="b2493-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="b2493-116">Restartujte prohlížeč Edge.</span><span class="sxs-lookup"><span data-stu-id="b2493-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="b2493-117">Přejděte na web, pro který máte nastavit indikátor.</span><span class="sxs-lookup"><span data-stu-id="b2493-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="b2493-118">Pokud se web nezobrazuje očekávaným způsobem, pokračujte krokem 3.</span><span class="sxs-lookup"><span data-stu-id="b2493-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="b2493-119">Krok 3: Shromažďování dat</span><span class="sxs-lookup"><span data-stu-id="b2493-119">Step 3: Collect data</span></span>

- <span data-ttu-id="b2493-120">Shromažďování **diagnostických dat MDEClientAnalyzer**</span><span class="sxs-lookup"><span data-stu-id="b2493-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="b2493-121">Pokyny najdete v tématu Problémy s zařízeními pro připojení k [Microsoft Defenderu pro koncový bod](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="b2493-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="b2493-122">Pokud máte s instalací a shromažďováním stop fiddlerů problémy, podívejte se na [stránku Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="b2493-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="b2493-123">Pokud upřednostňujete pokyny od podpory Microsoftu, vyberte níže ikonu Podpora a otevřete tak případ podpory.</span><span class="sxs-lookup"><span data-stu-id="b2493-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
