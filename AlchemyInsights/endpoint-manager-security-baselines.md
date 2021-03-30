---
title: EndPoint Manager – směrné plány zabezpečení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420773"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="2b757-102">EndPoint Manager – směrné plány zabezpečení</span><span class="sxs-lookup"><span data-stu-id="2b757-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="2b757-103">Směrné plány zabezpečení jsou předkonfigurované skupiny nastavení Windows, které vám pomůžou použít nastavení zabezpečení doporučená příslušnými týmy zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="2b757-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="2b757-104">Tyto směrné plány můžete přizpůsobit tak, aby doručili jenom požadovaná nastavení a hodnoty.</span><span class="sxs-lookup"><span data-stu-id="2b757-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="2b757-105">Další informace o směrných plánech zabezpečení najdete v článku Použití standardních hodnot zabezpečení ke konfiguraci zařízení [s Windows 10 v Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="2b757-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="2b757-106">V současné době existují směrné plány pro tyto produkty:</span><span class="sxs-lookup"><span data-stu-id="2b757-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="2b757-107">Nastavení zabezpečení Windows MDM</span><span class="sxs-lookup"><span data-stu-id="2b757-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="2b757-108">Microsoft Defender pro endpointové zabezpečení</span><span class="sxs-lookup"><span data-stu-id="2b757-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="2b757-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2b757-109">Microsoft Edge</span></span>

<span data-ttu-id="2b757-110">Každý směrný plán se pravidelně aktualizuje a vydává v přírůstkových verzích.</span><span class="sxs-lookup"><span data-stu-id="2b757-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="2b757-111">Každá verze přidá nebo odebere nastavení z předchozí verze, aby bylo zajištěno, že směrný plán splňuje aktuální pokyny.</span><span class="sxs-lookup"><span data-stu-id="2b757-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="2b757-112">Konzola Směrné plány zabezpečení v endpoint security umožňuje porovnání různých verzí tak, že zviditelníte změny z verze na verzi.</span><span class="sxs-lookup"><span data-stu-id="2b757-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="2b757-113">Pokyny, jak co nejúčinněji změnit, kterou verzi směrného plánu nasadíte, najdete v článku Správa standardních profilů zabezpečení [v Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="2b757-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="2b757-114">Po nasazení směrného plánu zabezpečení můžete sledovat stav nasazení a zkontrolovat nastavení podle zařízení.</span><span class="sxs-lookup"><span data-stu-id="2b757-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="2b757-115">**Poznámka:** Vykazování dat pro směrné plány může trvat až 24 hodin, než se zobrazí z příprava nasazení na zařízení a až 6 hodin pro další aktualizace.</span><span class="sxs-lookup"><span data-stu-id="2b757-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="2b757-116">Nejběžnější příčinou použití nastavení směrného plánu je to, že stejné nastavení se používá v jiném profilu.</span><span class="sxs-lookup"><span data-stu-id="2b757-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="2b757-117">Tento scénář můžete prozkoumat pro konkrétní zařízení tak, že toto zařízení vyberete z uzlu Stav zařízení v profilu Směrný plán zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="2b757-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="2b757-118">Podrobnosti najdete v tématu [Řešení konfliktů u směrných účaří zabezpečení](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="2b757-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>