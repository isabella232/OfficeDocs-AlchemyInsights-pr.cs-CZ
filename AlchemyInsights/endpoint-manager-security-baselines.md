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
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – Základní úrovně zabezpečení

Základní úrovně zabezpečení jsou předkonfigurované skupiny nastavení Windows, které vám pomůžou s používáním nastavení zabezpečení, jak je doporučují různé relevantní týmy zabývající se zabezpečením. Tyto základní úrovně si můžete přizpůsobit tak, aby zahrnovaly pouze vámi požadovaná nastavení a hodnoty. Další informace o základních úrovních zabezpečení najdete v tématu [Používání základních úrovní zabezpečení za účelem konfigurace zařízení s Windows 10 v aplikaci Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

V současnosti jsou k dispozici základní úrovně zabezpečení pro tyto produkty:

- Nastavení zabezpečení Windows MDM
- Zabezpečení Rozšířené ochrany před internetovými útoky v programu Microsoft Defender
- Microsoft Edge

Jednotlivé základní úrovně jsou pravidelně aktualizovány a vydávány v přírůstkových verzích. Každá verze přidává nebo odebírá nastavení z předchozí verze, aby základní úrověň nadále odpovídala současným požadavkům. Konzole základních úrovní zabezpečení v Zabezpečení koncového bodu umožňuje porovnání různých verzí, protože jsou změny provedené v jednotlivých verzích viditelné.

Návod, jak co nejefektivněji změnit, která verze bude nasazená, najdete v tématu [Správa profilů základních úrovní zabezpečení v aplikaci Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Po zavedení základní úrovně zabezpečení můžete monitorovat stav nasazení a kontrolovat nastavení na jednotlivých zařízeních.

**Poznámka:** Od prvotního zavedení na zařízení může trvat až 24 hodin, než se data generování sestav základní úrovně zabezpečení objeví. V případě dodatečných aktualizací to může trvat až šest hodin. 

Nejběžnější důvod, proč nejde základní úroveň zabezpečení použít, je souběžné používání stejného nastavení v jiném profilu. Tento scénář lze na vybraném zařízení ověřit, když zařízení vyberete z uzlu Stav zařízení v profilu Základní úrovně zabezpečení. Podrobnosti najdete v tématu [Řešení konfliktů základních úrovní zabezpečení](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).