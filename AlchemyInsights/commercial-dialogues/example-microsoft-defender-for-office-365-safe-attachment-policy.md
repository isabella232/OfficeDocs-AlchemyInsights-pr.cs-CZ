---
title: Příklad zásad bezpečné přílohy v Programu Microsoft Defender pro Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744525"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Příklad zásad bezpečné přílohy v Programu Microsoft Defender pro Office 365

Tato nastavení povolte zásadu *s* názvem Žádná zpoždění, která okamžitě doručí zprávy, a potom přílohy znovu připojte po jejich naskenování:

- **Název:** Bez zpoždění
- **Popis:** Doručuje zprávy okamžitě a znovu přichytá přílohy po skenování.
- **Odpověď:** Vyberte **možnost Dynamické doručení.** Další informace najdete v tématu [Dynamické doručování v zásadách bezpečných příloh](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Oddíl Příloha přesměrování:** Vyberte možnost Povolit přesměrování a zadejte e-mailovou adresu globálního správce Microsoftu 365, správce zabezpečení nebo analytika zabezpečení, který bude zkoumat škodlivé přílohy.
- **Oddíl Použitý na:** Vyberte **Doména příjemce je** a pak vyberte doménu. Vyberte **přidat** a pak vyberte **OK**. Po dokončení vyberte **Uložit**.

Další informace najdete v tématu [Bezpečné přílohy v programu Microsoft Defender pro Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
