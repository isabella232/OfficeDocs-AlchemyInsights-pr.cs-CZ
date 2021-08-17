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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889211"
---
# <a name="active-directory-not-syncing"></a>Active Directory se nesynchronuje

Pokud se vám zobrazí chyby synchronizace, například "žádná nedávná synchronizace", nebo si všimnete stavu synchronizace adresářů na portálu pro správu Office, že se jedná o poslední synchronizaci před více než 3 dny, může to být tím, že AADConnect má nesprávná nastavení nebo nedostatečná oprávnění k provedení synchronizace.  

Přeinstalace AADConnect pomocí expresního nastavení může problém rychle vyřešit:

1. [Stáhněte si nejnovější verzi AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Postupujte podle pokynů pro expresní instalaci](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Služba Azure AD Connect musí být nainstalovaná na Windows Serveru 2012 nebo novějším. Tento server musí být připojený k doméně a může to být řadič domény nebo členský server. Úplný seznam požadavků na služby Azure AD Připojení a předběžných požadavků naleznete v tématu Předpoklady pro [Azure AD Připojení](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Další informace o účtech služeb AADConnect najdete v tématu [Azure AD Připojení: Účty](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)a oprávnění .
