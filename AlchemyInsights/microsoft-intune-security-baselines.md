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
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886625"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Použití Microsoft Intune standardních hodnot zabezpečení ke konfiguraci Windows 10 zařízení

Standardní hodnoty zabezpečení Intune pomáhají chránit uživatele a zařízení. Směrné plány zabezpečení Windows předkonfigurované skupiny používané k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení. Vytvořením standardního profilu zabezpečení v Intune vytvoříte šablonu, která se skládá z více profilů konfigurace zařízení.

Když nasadíte standardní hodnoty zabezpečení do skupin uživatelů nebo zařízení, nastavení se použije na zařízeních, která běží Windows 10 nebo novějších verzích. Směrný plán zabezpečení microsoftu pro správu mobilních zařízení (MDM) například automaticky povolí nástroj BitLocker pro vyměnitelné jednotky, vyžaduje heslo pro odemknutí zařízení a zakáže základní ověřování. Pokud výchozí hodnota pro vaše prostředí nefunguje, můžete přizpůsobit směrný plán tak, aby se na vás šoustá nastavení, která potřebujete.

Standardní hodnoty zabezpečení také pomáhají vytvořit zabezpečený pracovní postup mezi koncovými Microsoft 365. Směrný plán zabezpečení obsahuje doporučené postupy a doporučení pro nastavení, která mají vliv na zabezpečení. Intune spolupracuje s týmem Windows zabezpečení, který vytváří směrné plány pro zásady skupiny, takže tato doporučení jsou založená na solidní pokyny a rozsáhlém prostředí.

Pokud intune ještě nevíte, kde začít, standardní hodnoty zabezpečení vám pomůžou rychle vytvořit a nasadit zabezpečený profil. Pokud aktuálně používáte zásady skupiny, migrace do Intune pro účely správy je mnohem jednodušší díky standardním hodnotám zabezpečení, protože jsou integrované do Intune a zahrnují špičkové možnosti správy.

Další informace najdete v článku [Windows standardních hodnot zabezpečení](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) a správy [mobilních zařízení](https://docs.microsoft.com/windows/client-management/mdm/).

