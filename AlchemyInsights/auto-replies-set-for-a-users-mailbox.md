---
title: Nastavení automatických odpovědí pro poštovní schránku
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
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046601"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Nastavení automatických odpovědí pro poštovní schránku uživatele

**Metoda 1**

1. Přihlaste se na portál Microsoftu 365.

2. Přejděte na **Uživatelé > Aktivní uživatelé** (nebo **Skupiny > Sdílené poštovní schránky**, pokud nastavujete sdílenou poštovní schránku).

3. Vyberte uživatele, který má poštovní schránku Microsoft Exchange.

4. V rozevírací nabídce vpravo přejděte na **Nastavení pošty > Automatické odpovědi** (pokud se jedná o sdílenou poštovní schránku, stačí v rozevírací nabídce kliknout na **Automatické odpovědi**).

**Metoda 2**

1. Přihlaste se k portálu pro správu Microsoftu 365 pomocí přihlašovacích údajů správce.

2. Rozbalte **Centra pro správu** a pak klikněte na **Exchange**.

3. V pravém horním rohu klikněte na obrázek, klikněte na **Jiný uživatel** a vyberte poštovní schránku uživatele, kterou chcete změnit.

4. Na levé straně vyberte **Možnosti**, klikněte na **Uspořádat e-mail** a pak klikněte na **Automatické odpovědi**.

**Metoda 3**

Spusťte v Exchange Online PowerShellu tuto rutinu:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Další informace o této rutině najdete v tématu [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
