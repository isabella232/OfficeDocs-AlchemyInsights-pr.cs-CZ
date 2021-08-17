---
title: Nástroj pro diagnostiku služby pro Windows virtuální plochu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052379"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Nástroj pro diagnostiku služby pro Windows virtuální plochu

Windows Virtuální plocha (WVD) nabízí diagnostický nástroj, který správcům umožňuje identifikovat chyby prostřednictvím jednoho rozhraní. Tento nástroj zaznamenává informace související s diagnostikou při každém použití funkce WVD někým, kdo má přiřazenou roli WVD. Každý protokol obsahuje informace o roli WVD, která je součástí aktivity, chybové zprávy, které se zobrazují během relace, a informace o tenantovi a uživateli. Azure Log Analytics můžete nakonfigurovat tak, aby zachycoval protokol aktivit vytvořený diagnostickým nástrojem. Postup:

1. Vytvořte pracovní prostor Log Analytics pomocí [portálu Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) nebo [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Připojení Windows do Azure Monitoru](https://go.microsoft.com/fwlink/?linkid=2129913). Získejte ID pracovního prostoru a primární klíč pracovního prostoru. Průvodce nastavením potřebuje tyto informace, aby mohl správně nakonfigurovat agenta a zajistit, aby mohl komunikovat s Azure Monitorem.
1. [Předáte diagnostická data do pracovního prostoru.](https://go.microsoft.com/fwlink/?linkid=2128284) Diagnostická data z tenanta WVD můžete předát do analýzy protokolů pro váš pracovní prostor.
1. [Identifikujte a diagnostikujte](https://go.microsoft.com/fwlink/?linkid=2128338) problémy, které jsou ve vztahu k WVD interní nebo externí.

Další informace o konfiguraci nástroje pro diagnostiku služby pro WVD najdete v tématu Použití [analýzy protokolů pro funkci diagnostiky.](https://go.microsoft.com/fwlink/?linkid=2128084)
