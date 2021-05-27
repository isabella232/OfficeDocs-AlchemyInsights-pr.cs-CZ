---
title: Pravidla pro omezení útoku na povrch
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676125"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="bc5f7-102">Pravidla pro omezení útoku na povrch</span><span class="sxs-lookup"><span data-stu-id="bc5f7-102">Attack surface reduction rules</span></span>

<span data-ttu-id="bc5f7-103">Vyloučení souborů nebo složek může výrazně omezit ochranu poskytovanou pravidly pro omezení útoku na povrch.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="bc5f7-104">Soubory, které by pravidlem blokovaly, se smí spouštět a žádná sestava ani událost se zaznamenávají.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="bc5f7-105">Vyloučení platí pro všechna pravidla, která výjimky povolují.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="bc5f7-106">Vyloučení funkce ASR používají stejnou syntaxi jako Antivirová ochrana v programu Microsoft Defender vyloučení.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="bc5f7-107">Podrobnosti najdete v tématu Konfigurace a ověření vyloučení pro [Antivirová ochrana v programu Microsoft Defender kontroly](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="bc5f7-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="bc5f7-108">Pokud se chcete vyhnout problémům, zkontrolujte Časté chyby, kterým se při [definování vyloučení vyhnout](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="bc5f7-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="bc5f7-109">Vyloučení nepodporují všechna pravidla asr.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="bc5f7-110">Pokud chcete ověřit, jestli vaše pravidlo podporuje vyloučení, podívejte se na tabulku Pravidla pro omezení povrchu [útoku](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="bc5f7-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="bc5f7-111">Pravidla pro omezení útoku na povrch</span><span class="sxs-lookup"><span data-stu-id="bc5f7-111">Attack surface reduction rules</span></span>

<span data-ttu-id="bc5f7-112">Útoková plocha vaší organizace zahrnuje všechna místa, kde by mohl útočník ohrozit zařízení nebo sítě organizace.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="bc5f7-113">Zmenšením útoku se rozumí ochrana zařízení a sítě organizace, takže útočníci mají méně způsobů, jak útoky provádět.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="bc5f7-114">Může vám pomoct konfigurace pravidel pro omezení povrchu útoku v Microsoft Defenderu pro koncový bod.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="bc5f7-115">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="bc5f7-115">For more information, see:</span></span>

- [<span data-ttu-id="bc5f7-116">Mapování identifikátoru GUID pravidla ASR na název</span><span class="sxs-lookup"><span data-stu-id="bc5f7-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="bc5f7-117">Požadavky na pravidla asr:</span><span class="sxs-lookup"><span data-stu-id="bc5f7-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="bc5f7-118">Windows 10 Pro verze 1709 nebo novější</span><span class="sxs-lookup"><span data-stu-id="bc5f7-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="bc5f7-119">Windows 10 Enterprise verze 1709 nebo novější</span><span class="sxs-lookup"><span data-stu-id="bc5f7-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="bc5f7-120">Windows Server, verze 1803 (půlroční kanál) nebo novější</span><span class="sxs-lookup"><span data-stu-id="bc5f7-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="bc5f7-121">Určení správného vyloučení, které se má použít</span><span class="sxs-lookup"><span data-stu-id="bc5f7-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="bc5f7-122">V protokolu Microsoft-Windows-Windows Defender/Operational vyhledejte id události 1121 nebo 1122.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="bc5f7-123">Vyhodnoťte scénář bloku a kontext a ověřte, že tento scénář je potřeba odblokovat.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="bc5f7-124">Přečtěte si hodnotu Path v podrobnostech události, což je hodnota, která definuje vyloučení.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="bc5f7-125">Vyloučení je co nejpřísnější.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="bc5f7-126">V případě potřeby použijte zástupný znak (například nahraďte uživatelskou proměnnou).</span><span class="sxs-lookup"><span data-stu-id="bc5f7-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="bc5f7-127">Použijte vyloučení podle potřeb nasazení.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="bc5f7-128">Podrobnosti najdete v tématu [Přizpůsobení pravidel pro omezení útoku na povrch](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="bc5f7-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="bc5f7-129">Vyloučení není poctěn</span><span class="sxs-lookup"><span data-stu-id="bc5f7-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="bc5f7-130">Určete, jestli pravidlo podporuje vyloučení.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="bc5f7-131">Podrobnosti najdete v článku [Pravidla pro omezení útoku na povrch](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="bc5f7-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="bc5f7-132">Zkontrolujte použité výjimky a ověřte pomocí dat události překlepy nebo špatně interpretované zástupné znaky.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="bc5f7-133">Další informace najdete v tématu [Podporované typy vyloučení.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="bc5f7-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="bc5f7-134">Pokud je vliv pravidla příliš vysoký, zvažte přesunutí pravidla (zpět) do režimu auditování a proveďte další ověření.</span><span class="sxs-lookup"><span data-stu-id="bc5f7-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="bc5f7-135">Podrobnosti najdete v tématu [otestování toho, jak fungují funkce Microsoft Defenderu](/microsoft-365/security/defender-endpoint/audit-windows-defender)pro koncové body v režimu auditování .</span><span class="sxs-lookup"><span data-stu-id="bc5f7-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="bc5f7-136">Pomocí tohoto příkazu můžete shromáždit data podpory a otevřít tak případ podpory:</span><span class="sxs-lookup"><span data-stu-id="bc5f7-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="bc5f7-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="bc5f7-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="bc5f7-138">Další informace najdete v tématu Problémy s zařízeními pro připojení k [Microsoft Defenderu pro koncové body](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="bc5f7-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
