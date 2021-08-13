---
title: Řešení potíží s accessem zamítl zprávy OneDrive pro firmy weby
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957786"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Řešení potíží s accessem zamítl zprávy OneDrive pro firmy weby

K tomuto problému nejčastěji dochází, když se uživatel odstraní a znovu vytvoří se stejným hlavním názvem uživatele( UPN). Nový účet se vytvoří pomocí jiné hodnoty PUID (Passport Unique ID). Když se uživatel pokusí získat přístup k kolekci webů nebo OneDrive, má uživatel nesprávný KÓD PUID. Druhý scénář zahrnuje synchronizaci adresářů s organizační jednotkou služby Active Directory (OU). Pokud se uživatelé už přihlásili k SharePoint a pak se přesunou do jiné OU a znovu se synchronizuje s SharePoint, může docházet k tomuto problému.

1. Chcete-li tento problém vyřešit, měli byste obnovit původní hlavní název uživatele pomocí kroků v článku Obnovení [uživatele v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Pokud nemůžete obnovit původního uživatele, měli byste odebrat starého uživatele z OneDrive pomocí těchto kroků, odeberte uživatele [ze seznamu informací o uživateli](). 
3. Až to bude hotové, můžete ověřit, že má uživatel práva správce k webu OneDrive, a to podle pokynů v článku Přidání správce pro uživatele [OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Další informace o úrovních oprávnění najdete v článku [Principy](https://docs.microsoft.com/sharepoint/understanding-permission-levels)úrovní oprávnění v SharePoint .
