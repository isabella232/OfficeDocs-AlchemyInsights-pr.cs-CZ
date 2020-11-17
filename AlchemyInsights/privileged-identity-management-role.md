---
title: Role správy privilegované identity
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088570"
---
# <a name="privileged-identity-managementpim-role"></a>Role správce privilegované identity

**Po aktivaci role nejsou udělována oprávnění**

Když aktivujete roli ve správě privilegované identity služby Azure AD (PIM), nemusí se aktivace okamžitě šířit na všechny portály, které vyžadují privilegovanou roli. Někdy se může stát, že se neprojeví změna, a to i v případě, že se změna šíří, ale ukládání do mezipaměti na portálu se nezmění.

Pokud je aktivace opožděná, postupujte takto:

1. Odhlaste se z portálu Azure a pak se znovu přihlaste. Když aktivujete roli Azure AD nebo roli prostředku Azure, uvidíte fáze aktivace. Po dokončení všech fází uvidíte odkaz odhlásit se. K odhlášení můžete použít tento odkaz. Tato akce vyřeší většinu případů pro zpoždění aktivace.
2. Ve PIM ověřte, že jste uvedeni jako člen role.
3. Pokud aktivujete roli správce Exchange, ujistěte se, že se odhlásíte a zase se přihlásíte. Pokud problém přetrvává, otevřete lístek podpory a vyvolejte ho jako problém. Pokud k centru zabezpečení a dodržování předpisů používáte roli správce Exchange, podívejte se na další krok.
4. Pokud aktivujete roli pro přístup k centru zabezpečení a dodržování předpisů nebo Pokud aktivujete roli správce SharePointu, dojde k některému zpoždění pro aktivaci až pár minut. Jedná se o známý problém a my aktivně pracujeme na řešení tohoto problému s těmito týmy.

Další informace najdete tady:

- [Aktivace mých rolí služby Azure AD v PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivace mých rolí zdrojů Azure v PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Po deaktivaci role nebo vypršení platnosti aktivace role nejsou oprávnění odebrána**

Když deaktivujete roli ve správě privilegované identity služby Azure AD nebo když vyprší lhůta pro její aktivaci, může dojít k prodlevě, po jejímž uplynutí budete mít přístup.

Pokud je deaktivace opožděná, postupujte takto:

1. Pokud jste deaktivaci role správce Exchange nebo uplynutím lhůty pro její aktivaci vyprší významné zpoždění před odebráním oprávnění, otevřete lístek podpory a sdělte pracovníkovi podpory, aby vám pomohli poznat lístek s privilegovanou správou přístupu (PAM) v Office o tomto problému.
2. Pokud vypršela lhůta pro aktivaci, ale máte pořád otevřenou relaci prohlížeče, zavřete prohlížeč. Roli můžete dál používat, dokud tuto relaci nezavřete. Jedná se o známý problém a my prohlížíme možnou opravu aktivně odvolat, jakmile vypršela platnost aktivace.

Pokud se vaše zpoždění liší od těchto dvou scénářů, otevřete lístek podpory.
