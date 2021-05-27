---
title: Pravidla pro omezení útoku na povrch
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676125"
---
# <a name="attack-surface-reduction-rules"></a>Pravidla pro omezení útoku na povrch

Vyloučení souborů nebo složek může výrazně omezit ochranu poskytovanou pravidly pro omezení útoku na povrch. Soubory, které by pravidlem blokovaly, se smí spouštět a žádná sestava ani událost se zaznamenávají. Vyloučení platí pro všechna pravidla, která výjimky povolují.

Vyloučení funkce ASR používají stejnou syntaxi jako Antivirová ochrana v programu Microsoft Defender vyloučení. Podrobnosti najdete v tématu Konfigurace a ověření vyloučení pro [Antivirová ochrana v programu Microsoft Defender kontroly](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Pokud se chcete vyhnout problémům, zkontrolujte Časté chyby, kterým se při [definování vyloučení vyhnout](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Vyloučení nepodporují všechna pravidla asr. Pokud chcete ověřit, jestli vaše pravidlo podporuje vyloučení, podívejte se na tabulku Pravidla pro omezení povrchu [útoku](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Pravidla pro omezení útoku na povrch

Útoková plocha vaší organizace zahrnuje všechna místa, kde by mohl útočník ohrozit zařízení nebo sítě organizace. Zmenšením útoku se rozumí ochrana zařízení a sítě organizace, takže útočníci mají méně způsobů, jak útoky provádět. Může vám pomoct konfigurace pravidel pro omezení povrchu útoku v Microsoft Defenderu pro koncový bod.

Další informace najdete tady:

- [Mapování identifikátoru GUID pravidla ASR na název](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Požadavky na pravidla asr:
    - [Windows 10 Pro verze 1709 nebo novější](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise verze 1709 nebo novější](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, verze 1803 (půlroční kanál) nebo novější](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Určení správného vyloučení, které se má použít

1. V protokolu Microsoft-Windows-Windows Defender/Operational vyhledejte id události 1121 nebo 1122.

1. Vyhodnoťte scénář bloku a kontext a ověřte, že tento scénář je potřeba odblokovat.

1. Přečtěte si hodnotu Path v podrobnostech události, což je hodnota, která definuje vyloučení.
    - Vyloučení je co nejpřísnější.
    - V případě potřeby použijte zástupný znak (například nahraďte uživatelskou proměnnou).

1. Použijte vyloučení podle potřeb nasazení. Podrobnosti najdete v tématu [Přizpůsobení pravidel pro omezení útoku na povrch](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Vyloučení není poctěn

1. Určete, jestli pravidlo podporuje vyloučení. Podrobnosti najdete v článku [Pravidla pro omezení útoku na povrch](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Zkontrolujte použité výjimky a ověřte pomocí dat události překlepy nebo špatně interpretované zástupné znaky. Další informace najdete v tématu [Podporované typy vyloučení.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Pokud je vliv pravidla příliš vysoký, zvažte přesunutí pravidla (zpět) do režimu auditování a proveďte další ověření. Podrobnosti najdete v tématu [otestování toho, jak fungují funkce Microsoft Defenderu](/microsoft-365/security/defender-endpoint/audit-windows-defender)pro koncové body v režimu auditování .

1. Pomocí tohoto příkazu můžete shromáždit data podpory a otevřít tak případ podpory:
    
   ** MDEClientAnalyzer.cmd -v**

    Další informace najdete v tématu Problémy s zařízeními pro připojení k [Microsoft Defenderu pro koncové body](issues-with-onboarding-machines.md).
