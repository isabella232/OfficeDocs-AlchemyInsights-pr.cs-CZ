---
title: Vytvoření skupiny
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088575"
---
# <a name="create-a-group"></a>Vytvoření skupiny

Toto téma popisuje vytvoření skupiny.

**Oprávnění k vytvoření skupiny**

Zkontrolujte, jestli máte oprávnění vytvořit novou skupinu. Globální správci můžou zakázat vytváření skupin na portálu Azure nebo v panelu přístup. Abyste mohli vytvořit novou skupinu nebo vám udělit odpovídající oprávnění, budete možná potřebovat správce.

**Správa oprávnění pro vytváření skupin**

1. Globální Správci mohou spravovat oprávnění k vytváření skupin (z bezpečnostních důvodů) nebo skupiny Office 365 vytvořené na portálu Azure Portal nebo v panelu přístup tak, že výběrem možnosti "uživatelé můžou vytvářet skupiny zabezpečení v portálech Azure" nebo "uživatelé můžou vytvářet skupiny Office **365 v Azure** portáls"  >  **(nastavení)**.
2. Pokud máte licenci Azure Active Directory P1 Premium, můžete vytvářet skupiny také pro výběr skupiny uživatelů.

**Zakázání uvítacího oznámení pro nové členy skupiny Office 365**

Uvítací oznámení, které se uživatelům přidají do skupin Office 365, můžete zakázat nastavením **UnifiedGroupWelcomeMessageEnabled** na false v PowerShellu. Přečtěte [si toto nastavení.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

