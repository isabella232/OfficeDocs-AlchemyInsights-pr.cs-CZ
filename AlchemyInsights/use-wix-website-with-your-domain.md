---
title: Používání WIX webu s zakoupeným nebo spravovaným systémem Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300691"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Používání WIX webu s zakoupeným nebo spravovaným systémem Office 365

- [Aktualizace záznamů DNS pro zachování vašeho webu u současného poskytovatele hostingu](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- WIX článek "připojení domény k WIX pomocí polohovací metody" doporučuje používat polohovací (přidání záznamů DNS na tento odkaz) namísto změny serverů s názvy při používání Office 365
- Pokud se i tak rozhodnete změnit názvové servery na WIX, budete muset  [vytvořit záznamy DNS na WIX pro Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Pokud byla vaše doména zakoupená od společnosti Microsoft, názvové servery se nedají změnit. Pokud budete muset změnit názvové servery, musel by být zakoupená doména společnosti Microsoft  [po 60 dnů předána jinému poskytovateli hostingu](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)