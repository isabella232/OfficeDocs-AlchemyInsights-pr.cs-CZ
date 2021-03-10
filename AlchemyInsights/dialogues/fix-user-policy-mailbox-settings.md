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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693303"
---
# <a name="fix-user-policymailbox-settings"></a>Oprava nastavení zásad uživatele/poštovní schránky

Tato zpráva se týká nastavení nevyžádané pošty v poštovní schránce. Nastavení si můžete zkontrolovat takto:

1. Spusťte prostředí Exchange Management Shell. Další informace najdete v článku [o otevření prostředí Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Spusťte tento příkaz (pomocí e-mailové adresy uživatele):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Zkontrolujte, jestli je e-mailová adresa odesílatele součástí **TrustedSendersAndDomains** nebo **BlockedSendersAndDomains.** Pokud je e-mailová adresa v jednom ze seznamů, budete ji možná muset odebrat. Další informace najdete v tématu [Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
