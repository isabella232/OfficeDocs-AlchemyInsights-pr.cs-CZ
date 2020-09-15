---
title: 618 zásady sdílení kalendáře
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684223"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Chyba zásad při sdílení kalendáře

1. Podle situace proveďte jednu z následujících akcí:
    - Připojení k Exchangi Online pomocí vzdáleného PowerShellu Další informace najdete v článku [připojení k Exchangi Online pomocí vzdáleného PowerShellu](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na místním serveru otevřete prostředí Exchange Management Shell.
2. Určete zásady sdílení přiřazené uživateli. To provedete tak, že spustíte následující příkaz a navrátili jste vrácenou zásadu:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualizace zásad sdílení pro uživatele Postupujte takto:
    - Otevřete centrum pro správu Exchange.
    - Klikněte na **organizace**a potom poklikejte na zásadu přiřazenou uživateli v části **individuální sdílení**. Toto je zásada vrácená v kroku 2.
    - Na stránce pravidlo sdílení vyberte úroveň sdílení kalendáře, kterou chcete povolit v části **Určete, jaké informace chcete sdílet**. klikněte na **Uložit**.

Další informace najdete v tématu: ["zásady neumožňují udělit oprávnění na této úrovni jednomu nebo více příjemcům při pokusu o sdílení kalendáře uživatelem](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
