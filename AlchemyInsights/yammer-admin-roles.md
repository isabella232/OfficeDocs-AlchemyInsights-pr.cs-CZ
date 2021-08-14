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
ms.openlocfilehash: a5d71f509b7006264b15549c7e8450d4ed7025b7dea3cfd80fe6f0fdf50b0b9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989692"
---
# <a name="about-yammer-admins"></a>O Yammer správců

**Správci sítě**

Globální správci jsou automaticky povýšeni na roli ověřeného správce v Yammer síti. V následujících případech se tato propagační akce nemusí vyskytnout správně:

- Existuje Yammer sítí a správce je přihlášený k nesprávnému. [Sloučení sítě](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) je nutné, abyste se k Yammer síti.
- Používá se Azure PIM. Uživatel nemusí být povýšen na globálního správce dost dlouho, aby k propagační akci došlo. Budoucí aktualizace systému Yammer tento problém vyřešit, ale je nejlepší, když uživatele povýšíte na globálního správce ručně.
- Problém se synchronizací existuje v Yammer síti. V takovém případě bude vyžadována žádost o podporu pro další vyšetřování.

Další informace o rolích Yammer najdete v tématu [Správa Yammer správců](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Správci skupin**

Správci skupin pro Microsoft 365 skupiny se synchronizují s členstvím ve skupině z Azure AD. U velkých skupin může tato synchronizace trvat delší dobu.
