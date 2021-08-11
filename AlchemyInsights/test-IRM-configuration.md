---
title: Testování konfigurace technologie IRM pro nové funkce OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812431"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testování konfigurace technologie IRM pro nové funkce OME

Pokud chcete ověřit, jestli je Microsoft 365 tenant nakonfigurovaný na používání nových funkcí OME, spusťte při připojení k Exchange Online [PowerShellu následující rutiny:](/powershell/exchange/exchange-online-powershell)


1. Zkontrolujte konfiguraci technologie IRM vašeho tenanta spuštěním `Get-IRMConfiguration` . Ujistěte se, že jsou tyto hodnoty nastavené na **Hodnotu True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Pomocí domény, adresy odesílatele a příjemce spusťte `Test-IRMConfiguration` . Pokud test neprojde, prohlédněte si konfiguraci technologie IRM.

Další informace o tom, jak ověřit konfiguraci technologie IRM, najdete v tématu Ověření nové konfigurace OME v [Exchange Online PowerShellu.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)