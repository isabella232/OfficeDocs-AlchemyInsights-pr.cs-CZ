---
title: Příklad zásad přílohy v programu Microsoft Defender Office 365 Sejf přílohy
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988288"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Příklad zásad přílohy v programu Microsoft Defender Office 365 Sejf přílohy

Tato nastavení povolte zásadu *s* názvem Žádná zpoždění, která okamžitě doručí zprávy, a potom přílohy znovu připojte po jejich naskenování:

- **Název:** Bez zpoždění
- **Popis:** Doručuje zprávy okamžitě a znovu přichytá přílohy po skenování.
- **Odpověď:** Vyberte **možnost Dynamické doručení.** Další informace najdete v tématu [Dynamické doručování v Sejf přílohy](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Oddíl Redirect attachment** (Přesměrovat přílohu): Vyberte možnost Povolit přesměrování Microsoft 365 a zadejte e-mailovou adresu globálního správce, správce zabezpečení nebo analytika zabezpečení, který bude zkoumat škodlivé přílohy. 
- **Oddíl Použitý na:** Vyberte **Doména příjemce je** a pak vyberte doménu. Vyberte **přidat** a pak vyberte **OK**. Po dokončení vyberte **Uložit**.

Další informace najdete v tématu [Sejf v programu Microsoft Defender pro Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
