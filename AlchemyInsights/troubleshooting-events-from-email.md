---
title: Odstraňování potíží s událostmi z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658727"
---
# <a name="troubleshooting-events-from-email"></a>Odstraňování potíží s událostmi z e-mailu

1. Ověřte, jestli je funkce pro poštovní schránku povolená: **Get- <mailbox> EventsFromEmailConfiguration-identity**

2. Potom se podívejte na události z e-mailu protokoly **exportovat – MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V protokolech události z e-mailu Najděte InternetMessageId, který odpovídá položce v poštovní schránce.  

4. TrustScore určuje, jestli je položka přidaná. Události budou přidány pouze v případě, že je TrustScore = "Trusted".

TrustScore je určený vlastnostmi SPF, DKIM nebo DMARC, které jsou v záhlaví zprávy.

Zobrazení těchto vlastností:

**Desktopová aplikace Outlook**

- Otevření položky
- Vlastnosti > souborů – > Internetová záhlaví

nebo

**MFCMapi**

- Přechod na položku ve složce Doručená pošta
- Vyhledejte PR_TRANSPORT_MESSAGE_HEADERS_W

Tyto vlastnosti se zjišťují a zaznamenávají při přenosu a směrování. Pro další řešení potíží možná budete muset zpracovat podporu přenosu o chybách v SPF, DKIM a. nebo DMARC.