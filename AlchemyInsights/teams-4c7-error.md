---
title: Chyba 4c7 v Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700196"
---
# <a name="4c7-error-in-microsoft-teams"></a>Chyba 4c7 v Microsoft Teams

K této chybě dochází, protože Microsoft Teams vyžaduje ověřování formulářů. Při nasazení služby AD FS (Active Directory Federation Services) není pro síť intranet ve výchozím nastavení povoleno ověřování pomocí formulářů. Pokud se integrované ověřování Windows nezdaří, zobrazí se výzva, abyste se přihlásili pomocí ověřování formulářů.

Tento problém vyřešíte tak, že povolíte ověřování pomocí formulářů v počítači s místní kopií služby Active Directory v konzole Microsoft Management Console (MMC) AD FS. Postupujte takto: 

1. V navigačním podokně přejděte na **zásady ověřování**.
2. V části **Akce** v podokně Podrobnosti vyberte **Upravit globální primární ověřování**.
3. Na kartě **intranet** vyberte **ověřování formulářů**.
4. Vyberte **OK** (nebo **použít**).