---
title: Nelze získat přístup k SharePointu nebo centru pro správu OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749471"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Nelze získat přístup k SharePointu nebo centru pro správu OneDrivu

- Pokud je váš web Centrum pro správu SharePointu nebo OneDrivu nedostupný nebo není dostupný, může se jednat o dočasný problém s tím, že uživatelé při přístupu k SharePointovým webům nebo obsahu OneDrivu dostanou přerušované zpoždění. Podívejte se na [řídicí panel stavu služeb](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) a zjistěte, jestli je vaše organizace ovlivněná.

- Globální a SharePointovým správcům musí být přiřazená licence na SharePoint. Nově vytvořené účty, které jsou právě přiřazené pomocí licence SharePointu nebo role správce, můžou mít problémy s přístupem k SharePointu, jako je "přístup odepřen" nebo "uživatel nebyl nalezen". K dokončení synchronizace v našem systému dejte alespoň 24 hodin. Chápeme, že 24 hodin se může jevit jako příliš dlouho. V mnoha případech jsme na řešení ještě pracujeme.

- Uživatelé správy identit ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) můžou mít přístup odepřený, pokud je v době, kdy je povolené accessové období velmi malé, informace  [o odepření přístupu k účtům PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).