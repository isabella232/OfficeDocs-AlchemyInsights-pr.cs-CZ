---
title: Synchronizace hesel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960828"
---
# <a name="password-synchronization"></a>Synchronizace hesel

**Synchronizace hodnot hash hesel vůbec nefunguje.**

Některé běžné problémy, se kterými se zákazníci setkávají, když synchronizace hodnot hash hesel nefunguje, jsou:

- Účtu služby Active Directory, který Azure AD Připojení používá ke komunikaci  s místní službou Active Directory, není udělena oprávnění Replikovat změny adresáře a Replikovat změny adresáře Všechna oprávnění, která jsou vyžadována pro synchronizaci hesel – je potřeba to vyřešit udělením těchto oprávnění účtu služby Active Directory. 
- Synchronizace hodnot hash hesel je zakázaná poté, co  správce změnil metodu User Sign-In z funkce Synchronizace hesel na jinou možnost, jako je  federace se službou **AD FS** v průvodci Azure AD Připojení – můžete to vyřešit tak, že znovu povolíte funkci synchronizace hodnot hash hesel v průvodci Azure AD Připojení.
- Problém s připojením k místní službě Active Directory Některé řadiče domény například nejsou přístupné službou Azure AD [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Připojení nebo jsou požadované porty bránou Firewall zablokované – Musíte to vyřešit tak, že zajistíte, že připojení mezi serverem Azure AD Připojení a místním adresářem Active Directory bude fungovat správně.
- Server Azure AD Připojení je momentálně v režimu pracovních úprav, což bude mít za následek, že server nebude moct mít přístup k hash hesel – Pokud chcete tento problém vyřešit, postupujte podle kroků popsaných v části Řešení synchronizace hesel se synchronizací [Azure AD Připojení –](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)žádná hesla se nesynchronují.

**Synchronizace hodnot hash hesel nefunguje pro některé z mých uživatelů**

1. Pokud jste si všimli, že se hodnota  hash hesla pro uživatele nesynchronuje, použijte k prošetření a vyřešení problému úlohu poradce při potížích Připojení Azure AD. Proveďte následující úkoly:

    a. [Spuštění úkolu poradce při potížích v průvodci](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Pomocí rutiny pro řešení potíží prošetřte problém se synchronizací hodnot hash hesel pro konkrétní použití.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Místní objekt uživatele služby Active Directory je pro uživatele povolený, musí při příštím **přihlášení** změnit heslo. Pokud je tato možnost povolená, uživateli se přiřadí dočasné heslo a při příštím přihlášení se zobrazí výzva ke změně hesla. Azure AD Připojení do Azure AD nesynchronuje dočasná hesla.

Pokud chcete vyřešit výše uvedený problém, proveďte některý z následujících úkolů:

- Požádejte uživatele, aby se přihlašuje k místní aplikaci (například Windows Desktop) a změnil heslo. Nové heslo se synchronizuje s Azure AD.
- Správce musí aktualizovat heslo uživatele bez povolení možnosti Uživatel musí při příštím přihlášení změnit heslo a nové heslo sdílet s uživatelem.

3. Místní objekt Uživatele služby Active Directory **není** správně nakonfigurovaný pro synchronizaci objektů nebo synchronizaci hesel. Pokud chcete tento problém vyřešit, postupujte podle kroků popsaných v tématu Poradce při potížích se synchronizací hodnot hash hesel [s Azure AD Připojení synchronizace](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







