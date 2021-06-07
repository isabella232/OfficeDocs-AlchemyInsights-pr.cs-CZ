---
title: Problémy s výkonem pro Microsoft Defender pro koncový bod v Linuxu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793638"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problémy s výkonem pro Microsoft Defender pro koncový bod v Linuxu

Tento článek vás provede kroky identifikace problémů s výkonem pro Microsoft Defender pro koncový bod v Linuxu.

Nejdřív je důležité ověřit, jestli je problém vyřešený v [nejnovější verzi](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Pokud chcete zahájit vyšetřování, podívejte se na článek Řešení problémů s [výkonem v Microsoft Defenderu pro koncový bod v Linuxu](/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Vyloučení

Vyloučení můžou pomoct zmírnit problémy s výkonem. Než začnete, zkontrolujte si vyloučení, aby bylo známé a zdokumentované jakékoli další riziko.

Další informace najdete v tématu Konfigurace a ověření vyloučení pro [Microsoft Defender pro koncový bod v Linuxu](/microsoft-365/security/defender-endpoint/linux-exclusions).

Pokud máte více souborů & složek, které chcete vyloučit, a všechny jsou na stejném přípojných bodech, může být jednodušší vyřadit přípojný bod. Počínaje únorovou verzí 101.22.80 můžete vyloučit celý mountpoint.

Pokud je například přípojný bod /mnt/backup, můžete do seznamu vyloučení přidat /mnt/backup spuštěním tohoto příkazu:

`$ mdatp exclusion folder add –path /mnt/backup`

**Poznámka:** Přidáním výjimek se zvyšuje riziko, že malware nebude detekován, a mělo by se s ním zacházet a implementovat opatrně.

## <a name="need-help"></a>Potřebujete pomoct?

Abyste vám pomohli co nejefektivnějším způsobem, shromážděte diagnostická data před otevřením případu podpory.
