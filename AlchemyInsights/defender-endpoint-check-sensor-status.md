---
title: Stav senzoru kontroly koncových bodů v programu Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676100"
---
# <a name="defender-endpoint-check-sensor-status"></a>Stav senzoru kontroly koncových bodů v programu Defender

Dlaždice **Zařízení s problémy se** senzorem je umístěná na řídicím panelu Operace zabezpečení. Tato dlaždice obsahuje informace o možnosti jednotlivých zařízení poskytovat data ze senzorů a komunikovat se službou Defender for Endpoint. Uvádí, kolik zařízení vyžaduje pozornost, a pomáhá vám identifikovat problematická zařízení a přijmout opatření k opravě známých problémů.

Dva indikátory stavu na dlaždici poskytují informace o počtu zařízení, která se službě nehladí správně:

- **Nesprávně nakonfigurované** Zařízení, která můžou částečně vykazovat data senzorů službě Defender for Endpoint a můžou mít chyby konfigurace, které je potřeba opravit.
- **Neaktivní** Zařízení, která přestala vykazovat službu Defender for Endpoint za poslední měsíc déle než sedm dní.

Kliknutím na libovolnou skupinu vás přesměruje na seznam Zařízení, který je filtrovaný podle vašich možností. V seznamu Zařízení můžete seznam stavu filtrovat podle následujícího stavu:

- **Aktivní** Zařízení, která aktivně hlásí službě Defender for Endpoint.
- **Nesprávně nakonfigurované** Zařízení, která můžou částečně vykazovat data senzorů službě Defender for Endpoint, ale mají chyby konfigurace, které je potřeba opravit. Nesprávně nakonfigurovaná zařízení mohou mít jeden nebo kombinaci následujících problémů:

    - Žádná data ze senzoru – Zařízení přestala odesílat data ze senzoru. Ze zařízení se pouštějí omezená upozornění.
    - Zhoršená komunikace – schopnost komunikovat se zařízením je zhoršená. Odesílání souborů pro hloubkovou analýzu, blokování souborů, izolování zařízení ze sítě a další akce, které vyžadují komunikaci se zařízením, nemusí fungovat.
- **Neaktivní** Zařízení, která přestala vykazovat zprávy službě Defender for Endpoint.

Pomocí funkce Exportovat si můžete stáhnout celý seznam ve formátu CSV.

Další informace najdete v tématu [Kontrola stavu senzoru v programu Microsoft Defender pro koncový bod](/microsoft-365/security/defender-endpoint/check-sensor-status).

Další informace o tom, co způsobilo, že zařízení bylo neaktivní nebo nesprávně nakonfigurované, najdete v článku Oprava chybných [senzorů](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)v Programu Microsoft Defender pro koncový bod .
