---
title: 2419 – nelze povolit – auditování
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767592"
---
# <a name="unable-to-enable-unified-auditing"></a>Nelze povolit jednotné auditování.

Když se pokusíte povolit jednotné auditování pro vaši organizaci, může se zobrazit chybová zpráva podobná této:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Tento problém vyřešíte takto:

1. [Připojení k PowerShellu služby Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Spusťte následující rutinu:

   ```
   Enable-OrganizationCustomization
   ```

3. Počkejte, až 60 minut, než se předchozí nastavení projeví.

4. Spusťte následující příkaz v online Exchangi PowerShellu:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Další informace najdete v následujících článcích:

- [Připojení k PowerShellu Exchange Online pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Zapnutí nebo vypnutí hledání v protokolu auditování](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
