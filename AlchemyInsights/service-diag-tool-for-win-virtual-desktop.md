---
title: Nástroj pro diagnostiku služeb pro virtuální plochu Windows
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677652"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Nástroj pro diagnostiku služeb pro virtuální plochu Windows

Virtual Desktop (WVD) systému Windows nabízí diagnostický nástroj, který správcům umožňuje identifikovat chyby prostřednictvím jednoho rozhraní. Tento nástroj slouží k protokolování informací o diagnostice, kdykoli WVD používá někdo přiřazený roli WVD. Každý protokol obsahuje informace o roli WVD zahrnuté v aktivitě, chybové zprávy, které se zobrazí během relace, a informace o tenantovi a uživateli. Analýzu protokolů Azure je možné nakonfigurovat tak, aby zachytával protokol aktivit vytvořený diagnostickým nástrojem. Postup:

1. Vytvořte pracovní prostor analýzy protokolů pomocí [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) nebo [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Připojte počítače se systémem Windows ke službě Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Získejte ID pracovního prostoru a primární klíč pracovního prostoru. Průvodce instalací potřebuje tyto informace, aby správně nakonfiguroval agenta a zajistil komunikaci s Azure monitorem.
1. [Zatlačte data diagnostiky do pracovního prostoru](https://go.microsoft.com/fwlink/?linkid=2128284). Data diagnostiky můžete zatlačit z tenanta WVD do analýzy protokolů pro váš pracovní prostor.
1. [Identifikujte a Diagnostikujte problémy](https://go.microsoft.com/fwlink/?linkid=2128338) , které jsou ve vztahu k WVD vnitřní nebo externí.

Další informace o konfiguraci nástroje pro diagnostiku služeb pro WVD najdete v tématu [použití funkce Analýza protokolů pro funkci diagnostiky](https://go.microsoft.com/fwlink/?linkid=2128084).
