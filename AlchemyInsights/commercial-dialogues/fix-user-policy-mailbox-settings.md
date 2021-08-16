---
title: Oprava nastavení zásad uživatele/poštovní schránky
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034711"
---
# <a name="fix-user-policymailbox-settings"></a>Oprava nastavení zásad uživatele/poštovní schránky

Tato zpráva se týká nastavení nevyžádané pošty v poštovní schránce. Nastavení si můžete zkontrolovat takto:

1. Spusťte Exchange Management Shell. Další informace najdete v [tématu Otevření Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Spusťte tento příkaz (pomocí e-mailové adresy uživatele):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Zkontrolujte, jestli je e-mailová adresa odesílatele součástí **TrustedSendersAndDomains** nebo **BlockedSendersAndDomains**. Pokud je e-mailová adresa v jednom ze seznamů, možná ji budete muset odebrat. Další informace najdete v tématu [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
