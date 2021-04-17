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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816341"
---
# <a name="create-a-group"></a>Vytvoření skupiny

Toto téma popisuje vytváření skupin.

**Oprávnění k vytvoření skupiny**

Ujistěte se, že máte oprávnění k vytvoření nové skupiny. Globální správci můžou vytváření skupin zakázat na portálu Azure portal nebo na přístupových panelech. Možná budete potřebovat správce, který za vás vytvoří novou skupinu nebo vám dá příslušná oprávnění.

**Správa oprávnění pro vytváření skupin**

1. Globální správci můžou spravovat oprávnění k vytváření skupin (z důvodů souvisejících se zabezpečením) nebo skupiny Office 365 vytvořené na portálu Azure portal nebo na accessových panelech tak, že zvolí "Uživatelé můžou vytvářet skupiny zabezpečení na portálech Azure" nebo "Uživatelé můžou vytvářet skupiny Office 365 na portálech Azure" v části Všechny skupiny – obecné  >  **(Nastavení)**.
2. Pokud máte licenci Azure Active Directory P1 Premium, můžete omezit vytváření skupin na výběr skupiny uživatelů.

**Zakázání uvítacího oznámení pro nové členy skupiny Office 365**

Uvítací oznámení odeslané uživatelům, kteří jsou přidáni do skupin Office 365, můžete zakázat nastavením **funkce UnifiedGroupWelcomeMessageEnabled** na False v PowerShellu. Další informace o tomto nastavení [najdete tady.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

