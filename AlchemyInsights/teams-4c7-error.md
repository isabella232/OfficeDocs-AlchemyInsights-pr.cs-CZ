---
title: Teams 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049301"
---
# <a name="4c7-error-in-microsoft-teams"></a>Chyba 4c7 v Microsoft Teams

K této chybě dochází, Microsoft Teams vyžaduje ověřování pomocí formulářů. Při nasazení služby AD FS (Active Directory Federation Services) není ověřování pomocí formulářů pro intranet ve výchozím nastavení povolené. Pokud Windows integrované ověřování selže, zobrazí se výzva k přihlášení pomocí ověřování pomocí formulářů.

Chcete-li tento problém vyřešit, povolte ověřování pomocí modulu snap-in KONZOLA MICROSOFT MANAGEMENT CONSOLE (MMC) služby AD FS v počítači, který má místní kopii služby Active Directory. Postupujte takto: 

1. V navigačním podokně přejděte na **Zásady ověřování**.
2. V **části Akce** v podokně podrobností vyberte Upravit globální primární **ověřování**.
3. Na kartě **Intranet** vyberte Ověřování **pomocí formulářů**.
4. Vyberte **OK** (nebo **Použít).**