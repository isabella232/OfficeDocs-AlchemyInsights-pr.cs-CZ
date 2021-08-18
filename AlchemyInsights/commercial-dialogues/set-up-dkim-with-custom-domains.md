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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332300"
---
# <a name="set-up-dkim-with-custom-domains"></a>Nastavení DKIM s vlastními doménami

Musíte publikovat dva záznamy CNAME pro každou vlastní doménu v DNS. K tomu použijte následující formát:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Poznámka:** **DomainGUID** je text nalevo od **.mail.protection.outlook.com** v přizpůsobených záznamech MX pro vlastní doménu (například contoso-com pro doménu **contoso.com).** **InitialDomain** je doména, kterou jste použili při Office 365 (například **contoso.onmicrosoft.com).**

Další informace o záznamech DNS najdete v tématu [Vytvoření záznamů DNS u libovolného](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)poskytovatele hostingu DNS pro Office 365 .