---
title: Použití standardních hodnot zabezpečení Microsoft Intune ke konfiguraci zařízení s Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50693416"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Použití standardních hodnot zabezpečení služby Microsoft Intune při konfiguraci zařízení s Windows 10

Standardní hodnoty zabezpečení Intune pomáhají chránit uživatele a zařízení. Směrné plány zabezpečení jsou předem nakonfigurované skupiny nastavení Windows používané k použití známé skupiny nastavení a výchozích hodnot doporučených příslušnými týmy zabezpečení. Vytvořením standardního profilu zabezpečení v Intune vytvoříte šablonu, která se skládá z více profilů konfigurace zařízení.

Když nasadíte standardní hodnoty zabezpečení pro skupiny uživatelů nebo zařízení, nastavení se použije na zařízeních s Windows 10 nebo novějších verzích. Například standardní hodnoty zabezpečení MDM (Mobile Device Management) microsoftu automaticky (1) umožňují nástroji BitLocker použít vyměnitelné jednotky, (2) vyžaduje heslo k odemknutí zařízení a (3) zakáže základní ověřování. Pokud ve vašem prostředí výchozí hodnota nefunguje, můžete přizpůsobit směrný plán a použít tak nastavení, která potřebujete.

Směrné plány zabezpečení taky pomáhají vytvořit v Microsoftu 365 zabezpečený pracovní postup od začátku do konce. Některé výhody této funkce jsou následující:
- Směrný plán zabezpečení zahrnuje doporučené postupy a doporučení pro nastavení, která mají vliv na zabezpečení. Protože Intune spolupracuje s týmem zabezpečení Windows, který vytváří standardní hodnoty pro zásady skupiny, jsou tato doporučení založená na solidní pokyny a rozsáhlém prostředí.
- Pokud Intune ještě nevíte, kde začít, standardní hodnoty zabezpečení vám pomůžou rychle vytvořit a nasadit zabezpečený profil.
- Pokud v současné době používáte zásady skupiny, je migrace na Intune pro účely správy mnohem jednodušší, protože tyto standardní hodnoty zabezpečení jsou integrované v Intune a zahrnují špičkové funkce pro správu.

Další informace najdete v [standardních hodnotách zabezpečení Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [a správě mobilních zařízení.](https://docs.microsoft.com/windows/client-management/mdm/)