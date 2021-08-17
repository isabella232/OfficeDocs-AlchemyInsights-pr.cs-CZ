---
title: Sada replik
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110673"
---
# <a name="replica-set"></a>Sada replik

AADDS se taky nazývá spravovaná doména. Jsou to vlastně dva řadiče domény, které back-end spouštěl a udržoval. Tyto dva řadiče domény zahrnují jeden hlavní řadič domény a jeden replikační řadič domény. Zálohy v AADDS (spravovaná doména) jsou automatizovaný proces spravovaný platformou Azure. V případě problému se spravovanou doménou vám může pomoct podpora Azure při obnovování ze zálohy.

Každou sadu replik vytvoříte ve virtuální síti. Každá virtuální síť musí být ve vzájemném vztahu ke každé jiné virtuální síti, která je hostitelem sady replik spravované domény. Tato konfigurace vytvoří síťovou topologii, která podporuje replikaci adresářů. Virtuální síť může podporovat více sad replik za předpokladu, že každá sada replik je v jiné virtuální podsíti.

Další podrobnosti o sadě replik najdete v tématu [Sady replik konceptů](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
