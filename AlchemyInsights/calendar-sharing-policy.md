---
title: Zásady sdílení kalendáře 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091591"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Chyba zásad při sdílení kalendáře

1. Podle situace proveďte jednu z těchto akcí:
    - Připojení k Exchange Online pomocí vzdáleného PowerShellu. Další informace najdete v tématu [Připojení Exchange Online vzdáleného PowerShellu](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na místním serveru otevřete Exchange Management Shell.
2. Určete zásady sdílení, které jsou přiřazené uživateli. Pokud to chcete udělat, spusťte následující příkaz a poznamenejte si vrácenou zásadu:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualizujte zásady sdílení pro uživatele. Postupujte takto:
    - Otevřete Centrum Exchange pro správu.
    - Klikněte **na** Organizace a potom poklikejte na zásadu přiřazenou uživateli v části **Individuální sdílení.** Toto je zásada vrácená v kroku 2.
    - Na stránce Pravidlo sdílení vyberte úroveň sdílení kalendáře, kterou chcete povolit v části Určení informací, **které chcete sdílet**; klikněte **na Uložit.**

Další informace najdete v článku o tom, že zásada neumožňuje udělit oprávnění na této úrovni jednomu nebo více příjemcům, když se uživatel pokusí sdílet [kalendář.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
