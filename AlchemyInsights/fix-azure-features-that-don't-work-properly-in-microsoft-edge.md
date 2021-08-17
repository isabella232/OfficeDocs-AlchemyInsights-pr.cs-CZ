---
title: Co dělat, když funkce Azure nefungují správně v Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117081"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Co dělat, když funkce Azure nefungují správně v Microsoft Edge

Microsoft Edge má [známé problémy,](https://go.microsoft.com/fwlink/?linkid=2140608) které souvisejí se zónami zabezpečení a můžou mít vliv na to, jak se uživatelé Azure přihlašují Windows Centra pro správu. Pokud máte problémy s používáním funkcí Azure s Microsoft Edge, vyzkoušejte následující postup:

1. V nabídce **Start** vyhledejte možnosti **Internetu** a vyberte ji.
2. V dialogovém **okně Vlastnosti** Internetu přejděte na **kartu** Zabezpečení.
3. Vyberte **zónu Důvěryhodné** weby a potom klikněte **na tlačítko** Weby.
4. V dialogovém **okně Důvěryhodné** weby přidejte i adresu URL brány a pak [https://login.microsoftonline.com](https://login.microsoftonline.com) vyberte [https://login.live.com](https://login.live.com) **Zavřít.**
5. V dialogovém **okně Vlastnosti** internetu přejděte na **kartu Ochrana** osobních údajů.
6. V části **Blokování automaticky otevíraných oken** vyberte **Nastavení**. V dialogovém okně, které se otevře, přidejte i adresu URL brány a [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) pak vyberte **Zavřít.**
