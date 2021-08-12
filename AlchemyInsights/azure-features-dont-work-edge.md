---
title: Co dělat, když funkce Azure nefungují správně v Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812863"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Co dělat, když funkce Azure nefungují správně v Microsoft Edge

Microsoft Edge má známé problémy související se zónami zabezpečení, které můžou mít vliv na to, jak se uživatelé Azure přihlašují Windows centra pro správu. Další informace najdete v článku [Známé problémy na Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Pokud máte problémy s používáním funkcí Azure s Microsoft Edge, zkuste toto:

1. Na nabídka Start na panelu **Hledání** zadejte Možnosti **Internetu** a vyberte ho.
1. V **okně Vlastnosti internetu** vyberte **kartu** Zabezpečení.
1. Vyberte **Důvěryhodné weby** a pak vyberte **Weby**.
1. Přidejte adresu URL brány a <https://login.microsoftonline.com> pak <https://login.live.com> a vyberte **Zavřít.**
1. V **okně Vlastnosti internetu** vyberte kartu **Ochrana** osobních údajů.
1. V části Blokování automaticky otevíraných oken vyberte **Nastavení**. Přidejte adresu URL brány a <https://login.microsoftonline.com> pak a pak vyberte <https://login.live.com> **Zavřít.**