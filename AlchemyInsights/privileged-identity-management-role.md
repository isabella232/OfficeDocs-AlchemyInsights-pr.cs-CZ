---
title: Privileged Identity Management role
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973222"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Oprávnění se neudělí po aktivaci role.**

Když aktivujete roli v Azure AD Privileged Identity Management (PIM), nemusí se aktivace okamžitě rozšířit na všechny portály, které vyžadují privilegované role. Někdy může dojít k tomu, že i když se změna rozšíří, může dojít k tomu, že ukládání do mezipaměti webu na portálu se okamžitě projeví.

Pokud je vaše aktivace zpožděná, postupujte takto:

1. Odhlásit se z portálu Azure Portal a pak se znovu přihlásit. Když aktivujete roli Azure AD nebo roli prostředků Azure, uvidíte fáze aktivace. Po dokončení všech fází se zobrazí odkaz Odhlásit se. Pomocí tohoto odkazu se můžete odhlásit. Ve většině případů se tím vyřeší zpoždění aktivace.
2. V aplikaci PIM ověřte, že jste uvedeni jako člen role.
3. Pokud aktivujete roli správce Exchange, ujistěte se, že se odhlásit a znovu přihlásit. Pokud problém potrvá, otevřete lístek podpory a vyděste ho jako problém. Pokud používáte roli správce Exchange přístup k Centru zabezpečení a dodržování předpisů, podívejte se na další krok.
4. Pokud aktivujete roli pro přístup k Centru zabezpečení a dodržování předpisů nebo pokud aktivujete roli správce SharePoint, dojde k nějakému zpoždění aktivace od několika minut až po několik hodin. Jedná se o známý problém a aktivně spolupracujeme s těmito týmy, aby tento problém co nejdříve vyřešili.

Další informace najdete tady:

- [Aktivace rolí Azure AD v pim](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivace rolí prostředků Azure v pim](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Oprávnění se odebrané po deaktivaci role nebo vypršení platnosti aktivace role**

Když deaktivujete roli ve službě Azure AD Privileged Identity Management nebo když vyprší doba aktivace role, může to být zpoždění, kdy budete mít dál přístup.

Pokud je deaktivace zpožděná, postupujte takto:

1. Pokud deaktivujete roli správce Exchange nebo vyprší doba aktivace role a všimnete si významného zpoždění před odebráním oprávnění, otevřete lístek podpory a řekněte technickému týmu podpory, aby vám pomohl se souborem lístku s týmem správy privilegovaného přístupu (PAM) uvnitř Office o tomto problému.
2. Pokud vypršela doba aktivace, ale pořád máte otevřenou relaci prohlížeče, zavřete prohlížeč. Roli můžete dál používat, dokud relaci nezadáte. Jedná se o známý problém a po vypršení platnosti aktivace se podíváme na potenciální opravu, která by aktivně odebrala jednotlivé relace.

Pokud se zpoždění liší od těchto dvou scénářů, otevřete lístek podpory.
