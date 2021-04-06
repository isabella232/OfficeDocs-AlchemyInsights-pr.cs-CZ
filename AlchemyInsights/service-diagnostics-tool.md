---
title: Nástroj pro diagnostiku služby pro virtuální plochu Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595517"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Nástroj pro diagnostiku služby pro virtuální plochu Windows

Windows Virtual Desktop (WVD) nabízí diagnostický nástroj, který správcům umožňuje identifikovat chyby prostřednictvím jednoho rozhraní. Tento nástroj zaznamenává informace související s diagnostikou při každém použití funkce WVD někým, kdo má přiřazenou roli WVD. Každý protokol obsahuje informace o roli WVD, která je součástí aktivity, chybové zprávy, které se zobrazují během relace, a informace o tenantovi a uživateli. Azure Log Analytics můžete nakonfigurovat tak, aby zachycoval protokol aktivit vytvořený diagnostickým nástrojem takto:

1. Vytvořte pracovní prostor Log Analytics pomocí [portálu Azure portal nebo](https://go.microsoft.com/fwlink/?linkid=2129500) Azure [PowerShellu.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Připojte počítače s Windows k Azure Monitoru.](https://go.microsoft.com/fwlink/?linkid=2129913) Získejte ID pracovního prostoru a primární klíč pracovního prostoru. Průvodce nastavením potřebuje tyto informace, aby mohl správně nakonfigurovat agenta a zajistit, aby mohl komunikovat s Azure Monitorem.

1. [Předáte diagnostická data do pracovního prostoru.](https://go.microsoft.com/fwlink/?linkid=2128284) Diagnostická data z tenanta WVD můžete předát do analýzy protokolů pro váš pracovní prostor.

1. [Identifikujte a diagnostikujte](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problémy, které jsou ve vztahu k WVD interní nebo externí.

Další informace o konfiguraci nástroje pro diagnostiku služby pro službu WVD najdete v tématu Použití analýzy protokolů pro funkci diagnostiky.