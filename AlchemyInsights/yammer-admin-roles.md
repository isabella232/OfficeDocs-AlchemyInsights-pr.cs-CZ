---
title: O Yammer správců
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/22/2021
ms.locfileid: "51035732"
---
# <a name="about-yammer-admins"></a>O Yammer správců

**Správci sítě**

Globální správci se automaticky propagují na roli ověřeného správce v Yammer síti. V následujících případech se tato propagační akce nemusí vyskytnout správně:

- Existuje Yammer sítí a správce je přihlášený k nesprávnému. [Sloučení sítě](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) je nutné, abyste se do jedné Yammer sítě.
- Používá se Azure PIM. Uživatel nemusí být povýšen na globálního správce dost dlouho, aby k propagační akci došlo. Budoucí aktualizace systému Yammer tento problém vyřešit, ale nejlepší je, když uživatele zvýšíte na globálního správce ručně.
- Se sítí Yammer existuje problém se synchronizací. V takovém případě bude vyžadována žádost o podporu pro další vyšetřování.

Další informace o rolích Yammer najdete v tématu [Správa Yammer správců](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Správci skupin**

Správci skupin pro skupiny připojené k Microsoftu 365 se synchronizují s členstvím ve skupině z Azure AD. U velkých skupin může tato synchronizace trvat delší dobu.
