---
title: Active Directory se nesynchronuje
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930968"
---
# <a name="active-directory-not-syncing"></a>Active Directory se nesynchronuje

Pokud se na portálu pro správu Office zobrazí chyby synchronizace, například "žádná nedávná synchronizace", nebo si všimnete stavu synchronizace adresářů na portálu pro správu Office, že se naposledy synchronizovala před více než 3 dny, může to být tím, že AADConnect má nesprávná nastavení nebo nemá dostatečná oprávnění k provedení synchronizace.  

Přeinstalace AADConnect pomocí expresního nastavení může problém rychle vyřešit:

1. [Stáhněte si nejnovější verzi AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Postupujte podle pokynů pro expresní instalaci](/azure/active-directory/hybrid/how-to-connect-install-express).

Služba Azure AD Connect musí být nainstalovaná na Windows Serveru 2012 nebo novějším. Tento server musí být připojený k doméně a může to být řadič domény nebo členský server. Úplný seznam požadavků na služby Azure AD Připojení a předběžných požadavků naleznete v tématu Předpoklady pro [Azure AD Připojení](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Další informace o účtech služeb AADConnect najdete v tématu [Azure AD Připojení: Účty](/azure/active-directory/hybrid/reference-connect-accounts-permissions)a oprávnění .
