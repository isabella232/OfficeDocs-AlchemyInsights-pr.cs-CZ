---
title: Konfigurace doménové služby
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884985"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nelze povolit AAD – DS nebo nasazení se nedaří.

Chcete-li vyřešit problém s povolením nebo selháním služby domény Azure AD (AAD-DS), proveďte následující kroky:

1. Pokud používáte už existující virtuální síť, zkontrolujte NSG pravidel, která blokují porty potřebné k synchronizaci v AAD-DS na portálu https://aka.ms/aadds-networking .
2. Zkontrolujte, jestli je v tomto průvodci odstraňováním potíží v téhle chybové zprávě odpověď, která je dostupná v  https://aka.ms/aadds-troubleshoot-enable .
3. Zkuste nasadit služby domény Azure AD v nové virtuální síti.
4. Postupujte podle pokynů Průvodce Začínáme s postupem nasazení [služby DNS](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Pokud máte problémy s nasazením služeb domény Azure AD, Projděte si téma [Poradce při potížích s doménami Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kde najdete běžné chyby, které vám pomůžou začít pracovat. 

**Nejde zakázat AAD – DS.**

AAD – DS nelze pozastavit. Pokud chcete spravovanou doménu přestat používat, musíte ji odstranit.
Pokud chcete odstranit spravovanou doménu, přečtěte si článek [odstranění služby DNS AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



