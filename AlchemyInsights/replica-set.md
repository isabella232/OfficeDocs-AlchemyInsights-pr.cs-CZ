---
title: Replikační sada
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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713496"
---
# <a name="replica-set"></a>Replikační sada

AADDS se taky nazývá spravovaná doména. Ve skutečnosti jde o dva řadiče domény, které provozuje a udržuje back-end. Tyto dvě počítače DCs zahrnují jednu hlavní dc a jednu replikační dc. Zálohy ve službě AADDS (spravovaná doména) jsou automatizovaný proces spravovaný platformou Azure. V případě problému se spravovanou doménou vám může pomoct podpora Azure při obnovování ze zálohy.

Každou sadu replik vytvoříte ve virtuální síti. Každá virtuální síť se musí vzájemně na partnerský vztah používat ke každé jiné virtuální síti, která hostuje replikační sadu spravované domény. Tato konfigurace vytvoří topologii sítě, která podporuje replikaci adresářů. Virtuální síť může podporovat několik sad replik za předpokladu, že je každá sada replik v jiné virtuální podsíti.

Další podrobnosti o sadě replik najdete v tématu Sady replik [konceptů.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
