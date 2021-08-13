---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007783"
---
# <a name="unable-to-enable-unified-auditing"></a>Jednotné auditování se nedaří povolit.

Když se pokusíte povolit jednotné auditování pro vaši organizaci, může se zobrazit chybová zpráva podobná následující:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Tento problém vyřešíte takto:

1. [Připojení k Exchange Online PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Spusťte následující rutinu:

   ```
   Enable-OrganizationCustomization
   ```

3. Počkejte 60 minut, než se projeví předchozí nastavení.

4. Spusťte následující příkaz v Exchange Online PowerShellu:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Další informace najdete v následujících článcích:

- [Připojení k Exchange Online PowerShellu pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Zapnutí nebo vypnutí vyhledávání v protokolu auditování](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
