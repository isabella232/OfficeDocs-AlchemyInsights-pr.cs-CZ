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
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – směrné plány zabezpečení

Směrné plány zabezpečení jsou předkonfigurované skupiny nastavení Windows, které vám pomůžou použít nastavení zabezpečení doporučená příslušnými týmy zabezpečení. Tyto směrné plány můžete přizpůsobit tak, aby doručili jenom požadovaná nastavení a hodnoty. Další informace o směrných plánech zabezpečení najdete v článku Použití standardních hodnot zabezpečení ke konfiguraci zařízení [s Windows 10 v Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

V současné době existují směrné plány pro tyto produkty:

- Nastavení zabezpečení Windows MDM
- Microsoft Defender pro endpointové zabezpečení
- Microsoft Edge

Každý směrný plán se pravidelně aktualizuje a vydává v přírůstkových verzích. Každá verze přidá nebo odebere nastavení z předchozí verze, aby bylo zajištěno, že směrný plán splňuje aktuální pokyny. Konzola Směrné plány zabezpečení v endpoint security umožňuje porovnání různých verzí tak, že zviditelníte změny z verze na verzi.

Pokyny, jak co nejúčinněji změnit, kterou verzi směrného plánu nasadíte, najdete v článku Správa standardních profilů zabezpečení [v Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Po nasazení směrného plánu zabezpečení můžete sledovat stav nasazení a zkontrolovat nastavení podle zařízení.

**Poznámka:** Vykazování dat pro směrné plány může trvat až 24 hodin, než se zobrazí z příprava nasazení na zařízení a až 6 hodin pro další aktualizace. 

Nejběžnější příčinou použití nastavení směrného plánu je to, že stejné nastavení se používá v jiném profilu. Tento scénář můžete prozkoumat pro konkrétní zařízení tak, že toto zařízení vyberete z uzlu Stav zařízení v profilu Směrný plán zabezpečení. Podrobnosti najdete v tématu [Řešení konfliktů u směrných účaří zabezpečení](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).