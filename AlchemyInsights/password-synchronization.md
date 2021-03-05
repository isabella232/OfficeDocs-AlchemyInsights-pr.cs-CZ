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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481143"
---
# <a name="password-synchronization"></a>Synchronizace hesel

**Synchronizace hodnot hash hesel nefunguje vůbec.**

K některým běžným problémům, se kterými se zákazníci setkávají, když synchronizace hodnot hash hesel nefunguje, jsou:

- Účet služby Active Directory používaný službou Azure AD Connect ke  komunikaci s místní  službou Active Directory nemá udělená oprávnění Replikovat změny adresáře a Replikovat změny adresáře – všechna oprávnění, která jsou potřeba pro synchronizaci hesel – musíte to vyřešit udělením těchto oprávnění účtu služby Active Directory.
- Synchronizace hodnot hash hesel je v průvodci Azure  AD Connect zakázaná poté, co správce změnil metodu Sign-In uživatele ze synchronizace hesel na jinou možnost, například Federování se službou **AD FS.** Můžete to vyřešit tak, že v průvodci Azure AD Connect znovu povolíte funkci synchronizace hodnot **hash** hesel.
- Potíže s připojením k místní službě Active Directory Některé řadičy domény například nejsou dostupné službou [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Connect nebo firewall zablokuje požadované porty – musíte to opravit tím, že zajistíte správné propojení mezi serverem Azure AD Connect a místní službou Active Directory.
- Server Azure AD Connect právě pracuje v režimu konfigurace, což by vedlo k tomu, že server nebude moct používat a hash hesel – pokud chcete tento problém vyřešit, postupujte podle kroků popsaných v části Řešení problémů se synchronizací hesel se synchronizací Azure AD Connect – žádná hesla se [synchronizují.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Některým uživatelům nefunguje synchronizace hodnot hash hesel**

1. Pokud jste zjistili, že se hodnota hash  hesel pro uživatele nesynchronuje, použijte k prozkoumání a vyřešení problému úlohu řešení potíží v Azure AD Connect. Proveďte následující úkoly:

    a. [Spuštění úkolu pro řešení potíží v průvodci](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Prozkoumejte problém se synchronizací hodnot hash hesel pro konkrétní použití pomocí rutiny pro řešení potíží.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Pro uživatele je povolený objekt místního uživatele služby Active Directory, musí **při** příštím přihlášení změnit heslo. Pokud je tato možnost povolená, přiřadí se uživateli dočasné heslo a při dalším přihlášení se zobrazí výzva ke změně hesla. Azure AD Connect nesynchronuje dočasná hesla se službou Azure AD.

Pokud chcete vyřešit výše uvedený problém, proveďte jednu z následujících akcí:

- Požádejte uživatele, aby se přihlašuje k místní aplikaci (třeba ke stolnímu počítači s Windows) a změnil heslo. Nové heslo se synchronizuje s Azure AD.
- Správce musí aktualizovat heslo uživatele, aniž by povolili možnost Uživatel musí při příštím přihlášení změnit heslo a nové heslo sdílet s uživatelem.

3. Místní objekt uživatele služby Active Directory **není** správně nakonfigurovaný na synchronizaci objektů nebo synchronizaci hesla. Pokud chcete tento problém vyřešit, postupujte podle kroků popsaných v tématu Řešení potíží se synchronizací hodnot hash hesel [se synchronizací Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







