---
title: Poradce při potížích s odepřením přístupu na weby OneDrivu pro firmy
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670609"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Poradce při potížích s odepřením přístupu na weby OneDrivu pro firmy

K tomuto problému dochází často, když se uživatel odstraní a znovu vytvoří se stejným hlavním názvem uživatele (UPN). Nový účet je vytvořen pomocí jiného identifikátoru PUID (kód účtu služby Passport). Když se uživatel pokusí získat přístup ke kolekci webů nebo k OneDrivu, má nesprávný PUID. Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory. Pokud se uživatelé už přihlásili k SharePointu a pak jsou přesunuti na jinou organizační jednotku a znovu se synchronizují se SharePointem, může dojít k těmto potížím.

1. Tento problém vyřešíte tak, že obnovíte původní název UPN pomocí kroků v článku [obnovení uživatele v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Pokud původního uživatele obnovit nemůžete, odeberte ho z webu OneDrivu tímto postupem tak, že [odeberete uživatele ze seznamu informace o uživateli](). 
3. Po dokončení této akce můžete ověřit, jestli má uživatel práva správce na web OneDrivu podle pokynů pro [Přidání správce na OneDrivu pro uživatele](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Další informace o úrovních oprávnění najdete v článku [Principy úrovní oprávnění v SharePointu](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
