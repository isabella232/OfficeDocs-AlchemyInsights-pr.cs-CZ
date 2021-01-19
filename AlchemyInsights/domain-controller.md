---
title: Řadič domény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900801"
---
# <a name="domain-controller"></a>Řadič domény

**Nelze povolit AAD – DS nebo nasazení se nedaří.**

Chcete-li vyřešit problém s povolením nebo selháním služby domény Azure AD (AAD-DS), proveďte následující kroky:

1. Pokud používáte už existující virtuální síť, zkontrolujte NSG pravidel, která blokují porty potřebné k synchronizaci v AAD-DS na portálu https://aka.ms/aadds-networking .
2. Zkontrolujte, jestli je v tomto průvodci odstraňováním potíží v téhle chybové zprávě odpověď, která je dostupná v  https://aka.ms/aadds-troubleshoot-enable .
3. Zkuste nasadit služby domény Azure AD v nové virtuální síti.
4. Postupujte podle pokynů Průvodce Začínáme s postupem nasazení služby AAD-DS, která je k dispozici v [kurzu vytváření služeb domény Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Pokud máte problémy s nasazením služeb domény Azure AD, Projděte si téma [Poradce při potížích s doménami Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kde najdete běžné chyby, které vám pomůžou začít pracovat. 

**Nejde zakázat AAD – DS.**

AAD – DS nelze pozastavit. Pokud chcete spravovanou doménu přestat používat, musíte ji odstranit.

Pokud narazíte na problémy, přečtěte si běžné chybové zprávy a související kroky řešení potíží, které vám pomůžou znovu začít pracovat, podívejte se na [řešení potíží se službou Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
