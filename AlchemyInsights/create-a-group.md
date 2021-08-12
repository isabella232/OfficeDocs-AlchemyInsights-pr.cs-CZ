---
title: Vytvoření skupiny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929298"
---
# <a name="create-a-group"></a>Vytvoření skupiny

Toto téma popisuje vytváření skupin.

**Oprávnění k vytvoření skupiny**

Ujistěte se, že máte oprávnění k vytvoření nové skupiny. Globální správci můžou vytváření skupin zakázat na portálu Azure portal nebo na přístupových panelech. Možná budete potřebovat správce, který za vás vytvoří novou skupinu nebo vám dá příslušná oprávnění.

**Správa oprávnění pro vytváření skupin**

1. Globální správci můžou spravovat oprávnění k vytváření skupin (z bezpečnostních důvodů Office 365) nebo skupiny vytvořené na portálu Azure portal nebo na přístupových panelech tak, že zvolí "Uživatelé můžou vytvářet skupiny zabezpečení na portálech Azure" nebo Office 365 "Uživatelé můžou vytvářet skupiny na portálech Azure" v části Všechny skupiny – obecné  >  **(Nastavení)**.
2. Pokud máte licenci na Azure Active Directory P1, můžete omezit vytváření Premium skupiny.

**Zakázání uvítacího oznámení pro nové Office 365 skupiny**

Uvítací oznámení odeslané uživatelům, kteří jsou přidáni do Office 365 skupin, můžete zakázat nastavením **funkce UnifiedGroupWelcomeMessageEnabled** na False v PowerShellu. Další informace o tomto nastavení [najdete tady.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

