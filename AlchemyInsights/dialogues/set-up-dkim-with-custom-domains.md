---
title: Nastavení DKIM s vlastními doménami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523684"
---
# <a name="set-up-dkim-with-custom-domains"></a>Nastavení DKIM s vlastními doménami

Pro každou vlastní doménu v DNS musíte publikovat dva záznamy CNAME. Můžete to udělat pomocí následujícího formátu:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** je text vlevo od **.mail.protection.outlook.com** v přizpůsobené mx záznamu pro vlastní doménu (například contoso-com pro doménu **contoso.com).** **InitialDomain** je doména, kterou jste použili při přihlášení k Office 365 (například **contoso.onmicrosoft.com).**

Další informace o záznamech DNS najdete v [článku Vytvoření ZÁZNAMŮ DNS pro Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)u libovolného poskytovatele hostingu DNS.