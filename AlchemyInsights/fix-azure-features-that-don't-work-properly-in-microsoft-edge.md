---
title: Co dělat, když funkce Azure v Microsoft Edge nefungují správně
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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583308"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Co dělat, když funkce Azure v Microsoft Edge nefungují správně

Microsoft Edge má [známé problémy](https://go.microsoft.com/fwlink/?linkid=2140608) související se zónami zabezpečení a může mít vliv na to, jak se uživatelé Azure přihlašují do centra pro správu Windows. Pokud máte v Microsoft Edge potíže s používáním funkcí Azure, vyzkoušejte následující postup:

1. V nabídce **Start** vyhledejte **Možnosti Internetu** a vyberte je.
2. V dialogovém okně **Internet – vlastnosti** přejděte na kartu **zabezpečení** .
3. Vyberte zónu **Důvěryhodné servery** a pak klikněte na tlačítko **weby** .
4. V dialogovém okně **Důvěryhodné servery** zadejte adresu URL brány [https://login.microsoftonline.com](https://login.microsoftonline.com) a taky a [https://login.live.com](https://login.live.com) pak vyberte **Zavřít**.
5. V dialogovém okně **Internet – vlastnosti** přejděte na kartu **soukromí** .
6. V části **blokování automaticky otevíraných oken** vyberte **Nastavení**. V dialogovém okně, které se otevře, přidejte adresu URL brány a taky [https://login.microsoftonline.com](https://login.microsoftonline.com) a [https://login.live.com](https://login.live.com) pak vyberte **Zavřít**.
