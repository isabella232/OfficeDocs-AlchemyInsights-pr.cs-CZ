---
title: Chyba Aplikace Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786662"
---
# <a name="4c7-error-in-microsoft-teams"></a>Chyba 4c7 v Microsoft Teams

K této chybě dochází, protože Microsoft Teams vyžaduje ověřování pomocí formulářů. Při nasazení služby AD FS (Active Directory Federation Services) není ověřování pomocí formulářů pro intranet ve výchozím nastavení povolené. Pokud se integrované ověřování ve Windows nepodaří, zobrazí se výzva k přihlášení pomocí ověřování pomocí formulářů.

Chcete-li tento problém vyřešit, povolte ověřování pomocí modulu snap-in KONZOLA MICROSOFT MANAGEMENT CONSOLE (MMC) služby AD FS v počítači, který má místní kopii služby Active Directory. Postupujte takto: 

1. V navigačním podokně přejděte na **Zásady ověřování**.
2. V **části Akce** v podokně podrobností vyberte Upravit globální primární **ověřování**.
3. Na kartě **Intranet** vyberte Ověřování **pomocí formulářů**.
4. Vyberte **OK** (nebo **Použít).**