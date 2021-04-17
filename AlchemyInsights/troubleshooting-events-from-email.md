---
title: Řešení potíží s událostmi z e-mailu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834832"
---
# <a name="troubleshooting-events-from-email"></a>Řešení potíží s událostmi z e-mailu

1. Ověřte, jestli je pro poštovní schránku povolená funkce: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Pak se podívejte na protokoly Události z **e-mailu Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V protokolech Události z e-mailu najděte Id internetové zprávy, které odpovídá položce v poštovní schránce.  

4. TrustScore určuje, jestli je položka přidaná nebo ne. Události se přidávají jenom v případě, že trustscore = "Důvěryhodný".

TrustScore je určeno vlastnostmi SPF, Dkim nebo Dmarc, které jsou v záhlaví zprávy.

Zobrazení těchto vlastností:

**Desktopový Outlook**

- Otevření položky
- File -> Properties -> Internet Headers

nebo

**KNIHOVNA MFCMapi**

- Přechod na položku ve složce Doručená pošta
- Hledejte PR_TRANSPORT_MESSAGE_HEADERS_W

Tyto vlastnosti se určují a zaznamenávají během přenosu a směrování. Pokud chcete další řešení potíží vyřešit, budete možná muset s podporou přenosu vyřešit chyby v SPF, DKIM a.nebo DMARC.