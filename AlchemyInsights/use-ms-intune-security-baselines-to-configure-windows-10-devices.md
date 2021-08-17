---
title: Použití Microsoft Intune standardních hodnot zabezpečení ke konfiguraci Windows 10 zařízení
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104337"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Použití Microsoft Intune standardních hodnot zabezpečení ke konfiguraci Windows 10 zařízení

Standardní hodnoty zabezpečení Intune pomáhají chránit uživatele a zařízení. Směrné plány zabezpečení Windows předkonfigurované skupiny nastavení používané k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení. Vytvořením standardního profilu zabezpečení v Intune vytvoříte šablonu, která se skládá z více profilů konfigurace zařízení.

Když nasadíte standardní hodnoty zabezpečení do skupin uživatelů nebo zařízení, použije se nastavení na zařízeních, která běží na Windows 10 nebo novějších zařízeních. Například mdm security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, (3) disables basic authentication. Pokud výchozí hodnota pro vaše prostředí nefunguje, přizpůsobte směrný plán tak, aby se na vás šoustá nastavení, která potřebujete.

Standardní hodnoty zabezpečení také pomáhají vytvořit zabezpečený pracovní postup mezi koncovými Microsoft 365. Tady jsou některé výhody:

- Směrný plán zabezpečení obsahuje doporučené postupy a doporučení pro nastavení, která mají vliv na zabezpečení. Vzhledem k tomu, že Intune spolupracuje s týmem Windows zabezpečení, který vytváří směrné plány pro zásady skupiny, jsou tato doporučení založená na solidní pokyny a rozsáhlém prostředí.
- Pokud intune ještě nevíte, kde začít, pak vám standardní hodnoty zabezpečení pomůžou rychle vytvořit a nasadit zabezpečený profil.
- Pokud v současné době používáte zásady skupiny, je migrace do Intune pro účely správy mnohem jednodušší díky standardním hodnotám zabezpečení, protože jsou integrované do Intune a zahrnují špičkové funkce pro správu.

Další informace najdete v článku [Windows standardních hodnot zabezpečení](https://go.microsoft.com/fwlink/?linkid=2141503) a správy [mobilních zařízení](https://go.microsoft.com/fwlink/?linkid=2141701).