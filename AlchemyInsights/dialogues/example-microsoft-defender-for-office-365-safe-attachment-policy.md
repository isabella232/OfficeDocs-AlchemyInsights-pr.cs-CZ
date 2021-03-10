---
title: Příklad zásady bezpečné přílohy v programu Microsoft Defender pro Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693103"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Příklad zásady bezpečné přílohy v programu Microsoft Defender pro Office 365

Toto nastavení umožňuje zásadu s názvem *Bez* zpoždění, která zprávy hned doručí a potom znovu naskenuje přílohy:

- **Název:** Bez zpoždění
- **Popis:** Zprávy se doručí okamžitě a znovu se naskenuje přílohy.
- **Odpověď:** Vyberte možnost **dynamického doručení.** Další informace najdete v článku [o dynamickém doručování v zásadách bezpečných příloh.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Část Přesměrovat** přílohu: Vyberte možnost povolit přesměrování a zadejte e-mailovou adresu globálního správce Microsoftu 365, správce zabezpečení nebo analytika zabezpečení, který bude prozkoumat škodlivé přílohy. 
- **Oddíl Použitý** na: **Vyberte doménu příjemce a** pak vyberte vaši doménu. Vyberte **Přidat a** pak vyberte **OK.** Až to budete mít, vyberte **Uložit.**

Další informace najdete v tématu Bezpečné [přílohy v programu Microsoft Defender pro Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
