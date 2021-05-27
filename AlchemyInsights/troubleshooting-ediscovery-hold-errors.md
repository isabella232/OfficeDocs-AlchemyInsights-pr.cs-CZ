---
title: Řešení potíží s ediscovery obsahuje chyby
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676083"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="016e6-102">Řešení potíží s ediscovery obsahuje chyby</span><span class="sxs-lookup"><span data-stu-id="016e6-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="016e6-103">Máte problémy s blokováním eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="016e6-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="016e6-104">Tady je několik doporučených postupů, které je třeba zvážit:</span><span class="sxs-lookup"><span data-stu-id="016e6-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="016e6-105">Zkontrolujte stav blokování distribuce.</span><span class="sxs-lookup"><span data-stu-id="016e6-105">Check the hold distribution status.</span></span>  <span data-ttu-id="016e6-106">Pokud je stav **Na (Čeká se)** nebo Vypnuto (čeká na **vyřízení),** počkejte, až se distribuce blokování dokončí.</span><span class="sxs-lookup"><span data-stu-id="016e6-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="016e6-107">Sloučení eDiscovery blokování aktualizací do jedné hromadné žádosti místo opakované aktualizace zásad pro každou transakci.</span><span class="sxs-lookup"><span data-stu-id="016e6-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="016e6-108">Spusťte Set-CaseHoldPolicy <policyname> -RetryDistribution v Powershellu Centra zabezpečení a dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="016e6-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="016e6-109">Podrobnosti najdete v tématu [Připojení k Centru & dodržování předpisů PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="016e6-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="016e6-110">Postup, jak zkontrolovat tato nastavení a další doporučené postupy pro zmírňování a řešení problémů s eDiscovery, najdete v tématu Řešení chyb blokování [eDiscovery](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="016e6-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="016e6-111">Informace o řešení jiných běžných problémů s eDiscovery najdete v tématu [Prošetřování,](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)odstraňování potíží a řešení běžných problémů s eDiscovery .</span><span class="sxs-lookup"><span data-stu-id="016e6-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
