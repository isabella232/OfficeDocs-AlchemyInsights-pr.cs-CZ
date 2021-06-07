---
title: Použití Microsoft Intune standardních hodnot zabezpečení ke konfiguraci Windows 10 zařízení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793614"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Použití Microsoft Intune standardních hodnot zabezpečení ke konfiguraci Windows 10 zařízení

Standardní hodnoty zabezpečení Intune pomáhají chránit uživatele a zařízení. Standardní hodnoty zabezpečení Windows předkonfigurovaných skupin používaných k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení. Vytvořením standardního profilu zabezpečení v Intune vytvoříte šablonu, která se skládá z více profilů konfigurace zařízení.

Když nasadíte standardní hodnoty zabezpečení do skupin uživatelů nebo zařízení, použije se nastavení na zařízeních, která běží na Windows 10 nebo novějších zařízeních. Směrný plán zabezpečení mdm (Microsoft Mobile Device Management) například automaticky povolí nástroj BitLocker vyměnitelných jednotek, vyžaduje heslo pro odemknutí zařízení a zakáže základní ověřování. Pokud výchozí hodnota pro vaše prostředí nefunguje, můžete přizpůsobit směrný plán tak, aby se na vás šoustá nastavení, která potřebujete.

Standardní hodnoty zabezpečení také pomáhají vytvořit zabezpečený pracovní postup mezi koncovými Microsoft 365. Směrný plán zabezpečení obsahuje doporučené postupy a doporučení pro nastavení, která mají vliv na zabezpečení. Intune spolupracuje s týmem Windows zabezpečení, který vytváří směrné plány pro zásady skupiny, takže tato doporučení jsou založená na solidní pokyny a rozsáhlém prostředí.

Pokud intune ještě nevíte, kde začít, standardní hodnoty zabezpečení vám pomůžou rychle vytvořit a nasadit zabezpečený profil. Pokud aktuálně používáte zásady skupiny, migrace do Intune pro účely správy je mnohem jednodušší díky standardním hodnotám zabezpečení, protože jsou integrované do Intune a zahrnují špičkové možnosti správy.

Další informace najdete v článku [Windows standardních hodnot zabezpečení](/windows/security/threat-protection/windows-security-baselines) a správy [mobilních zařízení](/windows/client-management/mdm/).

