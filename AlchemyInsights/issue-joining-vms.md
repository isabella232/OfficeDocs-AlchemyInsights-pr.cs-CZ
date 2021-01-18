---
title: Problém při připojování k VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884979"
---
# <a name="issue-joining-vms"></a>Problém při připojování k VMs

Pokud chcete vyřešit problémy, ke kterým dochází při připojování k virtuálním počítači, postupujte takto:

1. Zkuste se přihlásit pomocí formátu **UPN** (například ' joeuser@contoso.com ') místo formátu **sAMAccountName** (' CONTOSO\joeuser ').
2. Ujistěte se, že jste v souladu s postupem uvedeným v příručce *Začínáme* zapnutou funkci Synchronizace hesel.
3. Zkontrolujte, že daný uživatelský účet není externí účet v Azure AD. Externí uživatelé se nemohou přihlásit ke spravované doméně, protože doménové služby Azure AD neobsahují přihlašovací údaje těchto uživatelských účtů.
4. Pokud je ovlivněný uživatelský účet jenom Cloud, ujistěte se, že uživatelé změnili své heslo po tom, co jste povolili služby Azure AD. Tento krok způsobí vygenerování hodnot hash přihlašovacích údajů pro služby domény Azure AD.
5. Pokud se příslušné uživatelské účty synchronizují z místního adresáře, zkontrolujte, že je nakonfigurovaná doporučená verze Azure AD Connect, která provádí úplnou synchronizaci.
6. Pokud problémy přetrvávají po potvrzení kroku 4, proveďte z synchronizačního počítače následující příkazy:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.