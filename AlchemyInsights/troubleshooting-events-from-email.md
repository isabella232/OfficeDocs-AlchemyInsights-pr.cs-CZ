---
title: Poradce při potížích s událostmi z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568940"
---
# <a name="troubleshooting-events-from-email"></a>Poradce při potížích s událostmi z e-mailu

1. Ověřte, zda je funkce povolena pro poštovní schránku: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Pak se podívejte na 'Události z e-mailu' protokoly **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V protokolech Události z e-mailu najděte InternetMessageId, který odpovídá položce v poštovní schránce.  

4. TrustScore určuje, zda je položka přidána nebo ne. Události budou přidány pouze v případě, že TrustScore = "Trusted".

TrustScore je určena SPF, Dkim nebo Dmarc vlastnosti, které jsou v záhlaví zprávy.

Chcete-li zobrazit tyto vlastnosti:

**Outlook pro stolní počítače**

- Otevření položky
- File -> Vlastnosti -> Internet Záhlaví

nebo

**MFCMapi**

- Přechod na položku v doručené poště
- Podívejte se na PR_TRANSPORT_MESSAGE_HEADERS_W

Tyto vlastnosti jsou určeny a zaznamenány během přenosu a směrování. Pro další řešení potíží může být nutné sledovat s podporou přenosu o selhání v SPF, DKIM a.or DMARC.