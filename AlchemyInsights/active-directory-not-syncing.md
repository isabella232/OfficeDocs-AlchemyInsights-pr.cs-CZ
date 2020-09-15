---
title: Služba Active Directory se nesynchronizuje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697622"
---
# <a name="active-directory-not-syncing"></a>Služba Active Directory se nesynchronizuje

Pokud se vám zobrazují chyby synchronizace, třeba "žádná nedávná synchronizace" nebo se zobrazí stav synchronizace adresářů na portálu pro správu Office, znamená to, že se "naposledy synchronizace před více než 3 dny" znamená, že AADConnect má nesprávné nastavení nebo nemáte dostatečná oprávnění k provedení synchronizace.  

Přeinstalace AADConnect pomocí expresního nastavení se dá použít k rychlému vyřešení problému:

1. [Stáhněte si nejnovější verzi AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Postupujte podle pokynů pro expresní instalaci](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Další informace o účtech služeb AADConnect najdete v článku [Azure AD Connect: účty a oprávnění](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
