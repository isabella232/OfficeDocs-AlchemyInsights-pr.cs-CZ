---
title: EndPoint Manager – Základní úrovně zabezpečení
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440872"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="cb72e-102">EndPoint Manager – Základní úrovně zabezpečení</span><span class="sxs-lookup"><span data-stu-id="cb72e-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="cb72e-103">Základní úrovně zabezpečení jsou předkonfigurované skupiny nastavení Windows, které vám pomůžou s používáním nastavení zabezpečení, jak je doporučují různé relevantní týmy zabývající se zabezpečením.</span><span class="sxs-lookup"><span data-stu-id="cb72e-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="cb72e-104">Tyto základní úrovně si můžete přizpůsobit tak, aby zahrnovaly pouze vámi požadovaná nastavení a hodnoty.</span><span class="sxs-lookup"><span data-stu-id="cb72e-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="cb72e-105">Další informace o základních úrovních zabezpečení najdete v tématu [Používání základních úrovní zabezpečení za účelem konfigurace zařízení s Windows 10 v aplikaci Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="cb72e-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="cb72e-106">V současnosti jsou k dispozici základní úrovně zabezpečení pro tyto produkty:</span><span class="sxs-lookup"><span data-stu-id="cb72e-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="cb72e-107">Nastavení zabezpečení Windows MDM</span><span class="sxs-lookup"><span data-stu-id="cb72e-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="cb72e-108">Zabezpečení Rozšířené ochrany před internetovými útoky v programu Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="cb72e-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="cb72e-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="cb72e-109">Microsoft Edge</span></span>

<span data-ttu-id="cb72e-110">Jednotlivé základní úrovně jsou pravidelně aktualizovány a vydávány v přírůstkových verzích.</span><span class="sxs-lookup"><span data-stu-id="cb72e-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="cb72e-111">Každá verze přidává nebo odebírá nastavení z předchozí verze, aby základní úrověň nadále odpovídala současným požadavkům.</span><span class="sxs-lookup"><span data-stu-id="cb72e-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="cb72e-112">Konzole základních úrovní zabezpečení v Zabezpečení koncového bodu umožňuje porovnání různých verzí, protože jsou změny provedené v jednotlivých verzích viditelné.</span><span class="sxs-lookup"><span data-stu-id="cb72e-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="cb72e-113">Návod, jak co nejefektivněji změnit, která verze bude nasazená, najdete v tématu [Správa profilů základních úrovní zabezpečení v aplikaci Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="cb72e-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="cb72e-114">Po zavedení základní úrovně zabezpečení můžete monitorovat stav nasazení a kontrolovat nastavení na jednotlivých zařízeních.</span><span class="sxs-lookup"><span data-stu-id="cb72e-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="cb72e-115">**Poznámka:** Od prvotního zavedení na zařízení může trvat až 24 hodin, než se data generování sestav základní úrovně zabezpečení objeví. V případě dodatečných aktualizací to může trvat až šest hodin.</span><span class="sxs-lookup"><span data-stu-id="cb72e-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="cb72e-116">Nejběžnější důvod, proč nejde základní úroveň zabezpečení použít, je souběžné používání stejného nastavení v jiném profilu.</span><span class="sxs-lookup"><span data-stu-id="cb72e-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="cb72e-117">Tento scénář lze na vybraném zařízení ověřit, když zařízení vyberete z uzlu Stav zařízení v profilu Základní úrovně zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="cb72e-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="cb72e-118">Podrobnosti najdete v tématu [Řešení konfliktů základních úrovní zabezpečení](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="cb72e-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>