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
# <a name="troubleshooting-ediscovery-holds-errors"></a>Řešení potíží s ediscovery obsahuje chyby

Máte problémy s blokováním eDiscovery? Tady je několik doporučených postupů, které je třeba zvážit:

- Zkontrolujte stav blokování distribuce.  Pokud je stav **Na (Čeká se)** nebo Vypnuto (čeká na **vyřízení),** počkejte, až se distribuce blokování dokončí.
- Sloučení eDiscovery blokování aktualizací do jedné hromadné žádosti místo opakované aktualizace zásad pro každou transakci.
- Spusťte Set-CaseHoldPolicy <policyname> -RetryDistribution v Powershellu Centra zabezpečení a dodržování předpisů. Podrobnosti najdete v tématu [Připojení k Centru & dodržování předpisů PowerShell](/powershell/exchange/connect-to-scc-powershell).

Postup, jak zkontrolovat tato nastavení a další doporučené postupy pro zmírňování a řešení problémů s eDiscovery, najdete v tématu Řešení chyb blokování [eDiscovery](/microsoft-365/compliance/hold-distribution-errors).
Informace o řešení jiných běžných problémů s eDiscovery najdete v tématu [Prošetřování,](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)odstraňování potíží a řešení běžných problémů s eDiscovery .
